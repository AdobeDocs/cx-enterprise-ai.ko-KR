---
title: Agentic AI 사용 모니터링
description: CX Enterprise에서의 AI 사용량 모니터링을 위한 대시보드에 대해 알아봅니다. 채택률을 추적하고, 대화 및 피드백을 검토하고, 사용, 품질 및 비용 가시성에 대한 AI 크레딧을 관리합니다.
solution: Experience Cloud, Experience Platform
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
autotag-review: '2026-05-27T16:30:16.764Z'
TQID: 'https://experienceleague.adobe.com/J74yr0gGkFu1bzTmMvhrQ8TNaRX6nRjWY9WAwd3uydk'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
  - id: e1971122-7081-4556-9222-8a31bd71800c
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
subfeature_v2:
  - id: cda95149-19e1-4cfa-a57e-751283a32378
topic_v2:
  - id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8c
source-git-commit: a70c6440159ccb7c7544008da5707b23c42468cb
workflow-type: tm+mt
source-wordcount: 996
ht-degree: 1%

---

# Agentic AI 모니터링 대시보드

Agentic AI [!UICONTROL 모니터링] 대시보드는 COE(Center of Excellence) 구성원 및 기타 거버넌스 관련자들에게 Agentic AI 사용 및 채택에 대한 가시성을 제공합니다. [!DNL AI Assistant] 또는 다른 표면(예: [Adobe Marketing Agent for Microsoft 365 Copilot](https://experienceleague.adobe.com/ko/docs/cx-enterprise-ai/experience-cloud-ai/agents/ama-ms))을 사용하여 [!DNL Experience Platform Agents] 및 해당 사용자가 받는 값과 상호 작용하는 사용자를 보려면 7일 또는 30일 트렌드를 확인하십시오. 이러한 뷰를 함께 사용하면 가정 대신 데이터를 사용하여 에이전트 채택을 안내할 수 있습니다.

**가용성**

* 현재 하나 이상의 Experience Platform 기본 애플리케이션(Customer Journey Analytics, Journey Optimizer 또는 Real-Time CDP)에 대한 라이센스가 있는 모든 계정은 이 대시보드에 액세스할 수 있습니다
* Experimentation Accelerator, LLM Optimizer 및 Sites Optimizer과 같은 [AI 기반 응용 프로그램](agentic-ai.md#ai-first-cx-enterprise-applications)의 사용 및 채택 지표는 이 대시보드의 범위에 포함되지 않습니다.

[!UICONTROL 모니터링] 대시보드에는 다음 보기가 포함되어 있습니다.

| 대시보드 | 용도 |
| --- | --- |
| **개요** | 사용자, 대화, 피드백 및 신용 소모에 걸쳐 집계된 지표 |
| **사용자** | 사용자별 사용 빈도, 배포 및 참여 |
| **피드백** | 응답 품질 및 사용자 만족도에 대한 신호 |
| **AI 점수** | 신용 소비 추세 및 잔액 |

[Adobe CX Enterprise의 Agentic AI](agentic-ai.md) 설명서는 기존 CX Enterprise 앱의 [AI 에이전트](agentic-ai.md#existing-apps-table) 표에 사용 모니터링을 위한 범위 내의 에이전트를 나열합니다.

>[!VIDEO](https://video.tv.adobe.com/v/3491873?captions=kor&learn=on)

## 대시보드 권한 활성화 {#permissions}

승인된 각 사용자에 대한 제품 프로필 또는 역할을 업데이트하여 [!DNL Adobe Experience Platform]의 대시보드 액세스 권한을 부여합니다. [!UICONTROL 모니터링] 기능은 권한이 활성화된 후에 CX 엔터프라이즈 홈 페이지의 사용자에게 표시됩니다.

>[!IMPORTANT]
>
>모니터링 데이터는 기본 프로덕션 샌드박스에서만 사용할 수 있습니다. 개발 샌드박스는 모니터링 데이터를 보는 데 지원되지 않습니다. 사용자는 기본 프로덕션 샌드박스에 대해 필요한 모니터링 권한이 있어야 하며, 모니터링 데이터를 보려면 해당 샌드박스로 전환해야 합니다.
>
>혼동을 방지하기 위해 Adobe에서는 기본 프로덕션 샌드박스를 비롯한 모든 샌드박스에 대해 모니터링 권한을 부여하는 것이 좋습니다. 이렇게 하면 사용자가 현재 선택한 샌드박스에 관계없이 모니터링 대시보드에 액세스할 수 있으며 지원되지 않는 샌드박스를 빈 대시보드나 작동하지 않는 대시보드로 오인할 가능성을 줄일 수 있습니다.

**대시보드 권한을 활성화하려면**

1. [!DNL Experience Platform] **관리** > **권한**(으)로 이동합니다.

1. 업데이트할 제품 프로필 또는 역할을 엽니다.

   ![대시보드 권한 사용](assets/dashboards-permissions.png)

1. **[!UICONTROL AI Assistant]** 권한에서 **[!UICONTROL 리소스 추가]**&#x200B;를 클릭한 다음 **[!UICONTROL AI Assistant 사용 대시보드 보기]**&#x200B;를 활성화합니다.

   이 권한은 에이전트 AI 사용 모니터링 대시보드에 대한 액세스 권한을 부여합니다.

1. **[!UICONTROL 대시보드]** 권한에서 각 사용자의 권한에 따라 대시보드 액세스를 구성합니다.

   ![대시보드 권한 사용](assets/dashboards-add-resource.png)

   인증된 거버넌스 사용자에 대한 권장 권한:

   * **[!UICONTROL 라이선스 사용 대시보드 보기]**
   * **[!UICONTROL 표준 대시보드 보기]**
   * **[!UICONTROL 대시보드 데이터 내보내기]**(선택 사항, 승인된 거버넌스 사용자만 해당)

   필요한 경우 부여할 수 있는 추가 권한:

   * **[!UICONTROL 사용자 지정 대시보드 관리]**
   * **[!UICONTROL 사용자 지정 대시보드 보기]**
   * **[!UICONTROL 표준 대시보드 관리]**

1. 대시보드를 보려면 CX 엔터프라이즈 홈으로 돌아간 다음 **[!UICONTROL 모니터링]**&#x200B;을 클릭합니다.

   ![에이전트 AI 모니터링 대시보드](assets/monitoring.png)

## 개요 대시보드

개요 대시보드는 조직 전체의 채택 및 참여 지표를 위한 중앙 위치입니다. 이는 고도의 트렌드를 심층적인 분석으로 연결한다. 지표에 영향을 주는 요인을 보려면 모든 지표에서 개별 대화를 검토하십시오.

### 개요 대시보드의 지표

* **시간 경과에 따른 프롬프트:** 전반적인 사용 증가 및 채택 트렌드.
* **활성 사용자 및 대화:** [!DNL Experience Platform Agents]과(와) 상호 작용하는 사용자 수.
* **대화당 평균 프롬프트 수:** 대화당 참여 깊이.
* **피드백:** 사용자로부터의 엄지 손가락 위로 및 엄지 손가락 아래로 피드백 분포([!DNL AI Assistant] 상호 작용에만 해당).

>[!VIDEO](https://video.tv.adobe.com/v/3491883?captions=kor&learn=on)

### 대화 재생

대화 재생은 집계뿐만 아니라 개별 상호 작용을 보여줍니다. 많은 대화에 걸친 패턴을 분석하고 높은 수준의 트렌드에서 특정 대화로 이동할 수 있다.

* **프롬프트 및 응답 기록:** 사용자의 프롬프트 및 전달된 응답
* **피드백 신호:** 사용자가 마찰, 차단기 또는 사용 요구 사항을 식별하기 위해 엄지 손가락을 위로 또는 아래로 표시했습니다. 이 정보는 조직에서 신속한 관련성을 개선하는 데 도움이 되며 Adobe에서 시간이 지남에 따라 응답 품질을 개선하는 데 도움이 됩니다.

>[!VIDEO](https://video.tv.adobe.com/v/3491892?captions=kor&learn=on)

## 사용자 대시보드

사용자 대시보드에서는 에이전트 채택 및 참여가 시간에 따라 사용자마다 어떻게 달라지는지 보여줍니다. [!DNL Experience Platform Agents]을(를) 적극적으로 사용하는 사람과 사용하는 표면 및 참여 빈도를 확인할 수 있습니다. 관리자 및 COE 구성원은 개별 사용자 활동 및 대화를 드릴다운하여 참여 패턴 및 사용 동작을 이해할 수 있습니다.

### 사용자 대시보드의 지표

* **시간에 따른 채택 및 참여 트렌드:** 선택한 기간 동안 사용자 세그먼트가 어떻게 변경되는지 추적합니다. 사용자는 다음과 같이 분류됩니다.
  * **새로 만들기:** 선택한 기간의 첫 번째 활동으로 이전 12개월 동안 활동이 없습니다.
  * **반복:** 선택한 기간과 이전 기간의 활동입니다.
  * **선택한 기간에** 활동이 반환되지만 이전 기간에는 반환되지 않습니다.
  * **비활성:** 선택한 기간에는 활동이 없지만 이전 기간에는 활동이 있습니다.
* **사용자 참여 패턴:** 사용자가 에이전트와 상호 작용하는 빈도 및 시간이 지남에 따라 참여가 변경되는 방식.
* **대화 활동:** 사용자당 대화 및 프롬프트 수입니다.
* **상위 활성 사용자:** 참여도가 높은 사용자 및 팀이 에이전트 채택을 유도합니다.

>[!VIDEO](https://video.tv.adobe.com/v/3491925?captions=kor&learn=on)

## 피드백 대시보드

피드백 대시보드에는 에이전트 상호 작용에 대해 제출된 사용자 피드백이 표시됩니다. 사용자가 긍정적 또는 부정적으로 표시한 대화를 보고 피드백 이면의 상호 작용을 조사할 수 있다. 프롬프트, 응답, 추론 세부 정보 및 피드백 메모를 검토하려면 피드백 요약에서 개별 대화를 자세히 살펴보십시오.

### 피드백 대시보드의 지표

* **시간 경과에 따른 피드백 트렌드:** 시간에 따라 사용자 피드백이 변경되는 방식.
* **엄지손가락 위로 피드백 및 엄지손가락 아래로 피드백:** 양수 및 음수 상호 작용 신호.
* **피드백 범주:** 각 엄지손가락을 위로 올리고 아래로 내리는 이론적 근거입니다.
* **프롬프트 및 응답 기록:** 사용자 프롬프트 및 제출된 피드백과 관련된 응답.
* **피드백 세부 정보 및 메모:** 피드백을 제출하는 동안 사용자의 추가 컨텍스트 및 댓글입니다.

>[!VIDEO](https://video.tv.adobe.com/v/3491916?captions=kor&learn=on)

## AI 크레딧 대시보드

AI 크레딧 대시보드는 조직에서 [!DNL Experience Platform Agents]을(를) 사용하여 AI 크레딧 소비로 변환하는 방법을 보여 줍니다.

### AI 크레딧 대시보드의 지표

* **총 AI 크레딧 사용:** AI 크레딧의 전체 에이전트 사용.
* **일별 및 월별 트렌드:** 증가, 감소 및 소비 패턴의 변경.
* **남아 있는 AI 점수:** 잔액이 남아서 미리 계획을 세우고 초과 사용을 방지할 수 있습니다.

>[!VIDEO](https://video.tv.adobe.com/v/3491907?captions=kor&learn=on)

## 이 항목에 대한 추가 도움말

* [!DNL Experience Platform]의 [라이선스 사용 대시보드](https://experienceleague.adobe.com/ko/docs/experience-platform/dashboards/guides/license-usage)
* [Adobe CX Enterprise의 Agentic AI](agentic-ai.md)
* [에이전트 작업 및 AI 신용 소비](ai-credit-consumption.md)
* [라이선스 사용 대시보드](https://experienceleague.adobe.com/ko/docs/experience-platform/dashboards/guides/license-usage)&#x200B;(Experience Platform)
