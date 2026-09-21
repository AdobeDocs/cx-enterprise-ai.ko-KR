---
title: Adobe Experience Platform용 데이터 관리 에이전트
description: CX Coworker에서 데이터 관리 에이전트를 사용하여 Adobe Experience Platform 데이터 세트를 검색 및 분석하고 데이터 레이크 보존 정책을 관리하는 방법을 알아봅니다.
source-git-commit: 40f144c7a06592c78dccc6c17f19554b62f667c9
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 3%
---
# 데이터 관리 에이전트

>[!AVAILABILITY]
>
>데이터 관리 에이전트는 Adobe CX Enterprise Coworker에 대한 액세스 권한이 있는 모든 고객이 사용할 수 있습니다.

경험 이벤트 데이터 세트에 대한 데이터 레이크 보존을 이해하고 관리하려면 CX Coworker의 데이터 관리 에이전트를 사용합니다. Adobe Experience Platform 데이터 레이크의 Experience Event 데이터 세트가 증가하면 쿼리 및 다운스트림 프로세스를 완료하는 데 시간이 오래 걸리며 보존 요구 사항은 관리하기가 어려워질 수 있습니다. 당신이 성취하고자 하는 바를 자연어로 설명하세요. 데이터 관리 에이전트는 관련 Experience Event 데이터 세트를 찾고, 데이터 세트가 얼마나 활발하게 사용되는지 분석하며, 제안된 보존 기간이 미치는 데이터의 양을 모델링합니다. 작업을 수행할 준비가 되면 보존 정책을 설정, 변경 또는 제거하고 변경 사항이 발생하기 전에 확인을 요청하는 데 도움이 됩니다.

## 데이터 관리 에이전트에서 수행할 수 있는 작업 {#what-the-data-management-agent-can-do}

데이터 관리 에이전트는 4가지 기술을 제공합니다.

>[!NOTE]
>
>목록 데이터 세트, 데이터 세트 사용 분석 및 데이터 세트 유지 기술 분석은 읽기 전용입니다. 데이터 세트 보존 관리 기술만 데이터 레이크 보존 정책을 변경할 수 있으며 변경 사항을 적용하려면 먼저 명시적인 확인이 필요합니다.

| 스킬 | 설명 |
|---|---|
| **데이터 세트 나열** | 보존 검토를 시작할 위치를 결정할 때 사용합니다. 스토리지 크기, 행 수, 기존 보존 설정 및 프로필 활성화를 통해 경험 이벤트 데이터 세트를 나열하므로 데이터 레이크 보존 정책의 후보가 될 수 있는 데이터 세트를 빠르게 식별할 수 있습니다 |
| **데이터 집합 사용 분석** | 데이터 세트가 데이터 레이크 보존 정책에 적합한 후보인지 여부를 결정하기 전에 를 사용합니다. 최근 수집, 쿼리 활동 및 다운스트림 애플리케이션 사용과 같은 신호를 기반으로 특정 데이터 세트가 얼마나 적극적으로 사용되는지를 분류합니다. |
| **데이터 집합 보존 분석** | 보존 기간을 커밋하기 전에 를 사용합니다. 데이터 세트의 스토리지 지표와 데이터 보존 기간을 표시한 다음 해당 기간 분포를 사용하여 잠재적인 보존 기간이 유지하거나 제거할 데이터의 양을 근사화합니다. |
| **데이터 집합 보존 관리** | 행동할 준비가 되면 사용하십시오. 변경 전에 영향 미리보기 및 확인을 통해 데이터 세트에 대한 데이터 레이크 보존 정책을 설정, 변경 또는 제거합니다. |

## 범위: 데이터 레이크 보존과 기타 데이터 관리 도구 비교 {#scope}

경험 이벤트 데이터 세트를 검색 및 분석하고 데이터 레이크 보존 정책을 설정, 변경 또는 제거해야 하는 경우 데이터 관리 에이전트를 사용합니다.

데이터 레이크 보존 정책이 목표에 적합한 옵션인지 확실하지 않은 경우 [적합한 데이터 수명 주기 관리 기능 선택](https://experienceleague.adobe.com/ko/docs/experience-platform/data-lifecycle/choose-a-capability)을 참조하여 사용 가능한 보존 및 삭제 옵션을 비교하십시오.

이러한 기술은 다음과 같은 관련 기능을 관리하지 않습니다.

- **프로필 저장소 보존 정책.** 경험 이벤트가 프로필 저장소에 남아 있는 기간을 관리하려면 프로필이 활성화된 경험 이벤트 데이터 세트에 대한 경험 이벤트 만료 정책을 구성합니다. [경험 이벤트 만료](https://experienceleague.adobe.com/ko/docs/experience-platform/profile/event-expirations)를 참조하십시오.
- **샌드박스 전체의 익명 프로필 데이터 만료** 구성된 조건을 충족하면 샌드박스에서 익명 프로필 데이터를 자동으로 삭제하려면 [익명 프로필](https://experienceleague.adobe.com/ko/docs/experience-platform/profile/pseudonymous-profiles)을 참조하세요.
- **데이터 집합 만료.** 향후 날짜에 전체 데이터 집합을 삭제하도록 예약하려면 [데이터 집합 만료](https://experienceleague.adobe.com/ko/docs/experience-platform/data-lifecycle/ui/dataset-expiration)을 참조하세요.
- **레코드 삭제.** 개인 정보 보호 또는 위생상의 이유로 개별 프로필 레코드를 제거하려면 [레코드 삭제](https://experienceleague.adobe.com/ko/docs/experience-platform/data-lifecycle/ui/record-delete)를 참조하세요.

## 사전 요구 사항 {#prerequisites}

시작하기 전에 다음을 확인합니다.

- 검토할 데이터 세트가 포함된 Adobe Experience Platform 및 샌드박스에 대한 액세스 권한.
- 사용하려는 데이터 세트 및 보존 작업에 필요한 Adobe Experience Platform 권한입니다. 데이터 관리 에이전트는 기존 Experience Platform 권한을 사용하며 추가 액세스 권한을 부여하지 않습니다. Adobe Experience Platform 권한 및 역할의 작동 방식에 대한 자세한 내용은 [액세스 제어 개요](https://experienceleague.adobe.com/ko/docs/experience-platform/access-control/home)를 참조하세요.
- CX Coworker에 설치된 Adobe CXO 플러그인입니다.

플러그인 설치에 대한 지침은 [Coworker UI 안내서](https://experienceleague.adobe.com/ko/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide)를 참조하십시오.

## 데이터 관리 에이전트 사용 {#use-the-data-management-agent}

자연어를 사용하여 CX Coworker을 통해 데이터 관리 에이전트와 상호 작용합니다. 목표를 설명한 다음 후속 질문을 통해 결과를 구체화합니다.

>[!NOTE]
>
>시작하기 전에 검토할 데이터 세트가 포함된 샌드박스에서 작업 중인지 확인하십시오.

데이터 관리 에이전트를 사용하려면:

1. **[!UICONTROL CX Coworker]**(으)로 이동합니다. 액세스 세부 정보는 [Coworker UI 안내서](https://experienceleague.adobe.com/ko/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide)를 참조하십시오.
1. 수행할 작업을 설명하는 요청을 입력합니다.
1. 결과를 검토하고 후속 질문을 사용하여 조사를 계속합니다.

요청이 데이터 레이크 보존 정책을 변경하는 경우 데이터 관리 에이전트에는 제안된 영향이 표시되며 변경 사항을 적용하기 전에 확인해야 합니다.

데이터 세트를 식별하고, 사용 및 보존 영향을 분석하고, 데이터 레이크 보존 정책을 관리하는 전체 워크플로에 대해서는 [데이터 레이크 보존 관리](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md)를 참조하십시오.

## 데이터 관리 에이전트 작동 방식 {#how-the-data-management-agent-works}

데이터 관리 에이전트는 결정론적 계산을 사용하여 데이터 세트 사용을 분석하므로 동일한 입력이 동일한 사용 계층을 생성합니다. 또한 AI가 생성한 추정치에 의존하지 않고 프로그래밍 방식으로 유지 영향을 계산합니다. 유지 영향은 데이터의 연령 분포를 기반으로 하므로 근사치로 유지됩니다. 에이전트는 Adobe Experience Platform 서비스에서 직접 데이터를 검색하여 데이터 세트에 대한 현재 정보를 제공합니다.

## 제한 사항 {#limitations}

데이터 관리 에이전트는 데이터 레이크 보존 정책에 좋은 후보일 수 있는 데이터 세트를 식별할 수 있지만 데이터 세트에 데이터 세트가 필요한지 여부는 결정하지 않습니다. 명시적인 확인 없이 보존 정책을 적용, 변경 또는 제거하지 않습니다.

## 다음 단계 {#next-steps}

각 스킬을 사용하여 경험 이벤트 데이터 세트에서 데이터 레이크 보존을 검색, 분석 및 관리하는 방법에 대한 지침은 [데이터 레이크 보존 관리](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md)를 참조하십시오.

보존 동작 및 구성을 포함하여 Adobe Experience Platform에서 데이터 레이크 보존 정책이 작동하는 방법에 대한 자세한 내용은 [경험 이벤트 TTL(데이터 세트 보존) 안내서](https://experienceleague.adobe.com/ko/docs/experience-platform/catalog/datasets/experience-event-dataset-retention-ttl-guide)를 참조하십시오.
