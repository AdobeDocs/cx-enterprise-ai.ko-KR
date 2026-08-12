---
description: 데이터 인사이트, 대상, 여정 및 플랫폼 작업에서 영역별로 구성된 동료 채팅 사용 사례와 샘플 프롬프트를 찾아봅니다.
title: 동료 채팅 사용 사례
source-git-commit: 8a6d1c51abb7702298af4ac294dbe96a3b90e2df
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 4%

---

# 동료 채팅 사용 사례{#use-cases}

공동 작업자 채팅을 사용하면 여러 UI를 탐색하거나 수동으로 쿼리를 작성하는 대신 자연어를 사용하여 [!DNL Experience Platform] 데이터를 쿼리하고, 분석하고, 작업할 수 있습니다. 이 페이지에는 데이터 통찰력, 대상, 여정, 기본 요소 및 샌드박스 툴과 같이 작업 영역별로 구성된 사용 사례 전문가가 가장 많이 사용하는 카탈로그가 포함되어 있습니다. 각 항목에는 호출하는 스킬, 함께 작동하는 애플리케이션, 복사, 자체 데이터에 맞게 조정 및 대화를 통해 구체화할 수 있는 샘플 프롬프트가 포함됩니다.

## 데이터 인사이트

| 사용 사례 | 설명 | 스킬 | 애플리케이션 | 샘플 프롬프트 |
| --- | --- | --- | --- | --- |
| [CJA 보고서 및 지표 가져오기](data-insights/analytics-chat.md) | 실시간으로 CJA을 쿼리하여 지표, 차원, 세그먼트 및 데이터 보기를 가져옵니다. | `cja` | Customer Journey Analytics(CJA) | &quot;지난 30일 동안의 페이지 보기 횟수 표시&quot; · &quot;마스터 데이터 보기에 상위 세그먼트 나열&quot; |
| 비교 분석 | 채널, 기간 또는 세그먼트 간에 지표를 나란히 비교 | `cja` | Customer Journey Analytics(CJA) | &quot;월별 채널별 매출 비교&quot; · &quot;이번 분기에 모바일과 데스크탑 간 전환은 어떻게 보입니까?&quot; |
| Funnel 분석 | 각 단계에서 드롭오프로 여러 단계의 전환 단계를 거칩니다. | `cja` | Customer Journey Analytics(CJA) | &quot;체크아웃 funnel 안내&quot; · &quot;PDP에서 구매로 변환 funnel 표시&quot; |
| 예측 | 내역 CJA 데이터를 기반으로 향후 지표 값 프로젝트 | `cja` | Customer Journey Analytics(CJA) | &quot;향후 30일 동안의 세션 예측&quot; · &quot;매출 목표를 달성할 수 있습니까?&quot; |
| [근본 원인 분석](data-insights/root-cause-analysis.md) | 지표가 변경된 이유를 조사합니다. 드롭, 스파이크 및 예외 항목을 진단합니다. | `cja-root-cause-analysis` | Customer Journey Analytics(CJA) | &quot;지난 주에 전환율이 떨어진 이유는 무엇입니까?&quot; · &quot;1월 15일 매출 급증의 원인은 무엇입니까?&quot; |
| 경영진 요약 및 KPI 다이제스트 | 이해 당사자에게 준비된 성능 요약, 규범적 권장 사항 및 슬라이드 데크 개요 작성 | `cja-executive-summary` | Customer Journey Analytics(CJA) | &quot;지난달 요약 제공&quot; · &quot;이번 분기 데이터를 활용하여 슬라이드 데크 개요 만들기&quot; |
| [AA ↔ CJA 데이터 유효성 검사](data-insights/data-validation-aa-cja.md) | Adobe Analytics과 Customer Journey Analytics 간의 데이터 비교, 감사 및 조정 | `aa-cja-validation` | ADOBE ANALYTICS + CJA | &quot;AA 보고서 세트를 내 CJA 데이터 보기 비교&quot; · &quot;AA와 CJA 간의 페이지 보기 유효성 검사&quot; |
| 운영 시계열 및 인과관계 분석 | 인과 관계 속성을 사용하여 대상자, 데이터 세트 및 여정에 대한 내역 시계열 데이터를 쿼리하고 분석합니다. | `operational-stats-causal-analysis` | 모든 적격 지원 | &quot;지난 90일 동안의 대상 크기 트렌드를 표시합니다.&quot; · &quot;3월 3일에 데이터 세트 행 수가 급증한 이유는 무엇입니까?&quot; |
| 사용자 지정 CJA 스킬 만들기 | 분석 패턴을 세션 간에 지속되는 재사용 가능한 반복 가능한 스킬로 변환 | `cja-skill-creator` | Customer Journey Analytics(CJA) | &quot;이 주간 수익 분석을 재사용 가능한 스킬로 전환&quot; · &quot;월별 funnel 보고를 위한 스킬로 저장&quot; |

## 대상자

| 사용 사례 | 설명 | 스킬 | 애플리케이션 | 샘플 프롬프트 |
| --- | --- | --- | --- | --- |
| [자연어에서 대상 만들기](audiences/create-audience-from-natural-language.md) | 각 단계에서 사용자 승인을 통해 단계별 대상 만들기 오케스트레이션 | `audience-creation-flow` | Real-Time CDP(RTCDP) | &quot;지난 30일 동안 구매한 사용자 대상 만들기&quot; · &quot;캘리포니아에서 가치가 높은 충성도 구성원을 위한 세그먼트 만들기&quot; |
| PQL 정의 작성 | XDM 속성, 동작 이벤트 또는 기존 대상에서 대상 정의를 조합하고 집계 및 시간 창을 지원합니다. | `segment-definition-assembly` | Real-Time CDP(RTCDP) | &quot;3개 이상의 제품을 보았지만 구매하지 않은 사용자를 위한 PQL 만들기&quot; · &quot;내 이벤트 상태에 7일 기간 추가&quot; |
| 대상자 검색 및 찾기 | ID, 이름, 의미 체계 검색으로 대상 찾기, 중복 감지 및 중복 분석 | `audience-search` | Real-Time CDP(RTCDP) | &quot;모든 충성도 대상 찾기&quot; · &quot;내 &#39;휴일 쇼핑객&#39; 세그먼트가 중복됩니까?&quot; |
| 대상 크기 예상 | 폴링과 함께 Adobe Experience Platform 미리보기 API를 사용하여 PQL 표현식에 대한 프로필 도달 예상 | `audience-size-estimate` | Real-Time CDP(RTCDP) | &quot;이 대상자의 크기는 얼마나 됩니까?&quot; · &quot;이 PQL 표현식에 대한 도달 범위 예상&quot; |
| 대상자 크기 폭포 | PQL을 하위 술어로 분해하고 각 조건이 최종 대상 크기에 기여하는 방식을 표시합니다 | `audience-size-waterfall` | Real-Time CDP(RTCDP) | &quot;이 PQL의 폭포를 보여 주십시오.&quot; · &quot;각 조건이 대상자를 어떻게 감소시키는지 분류하십시오.&quot; |
| 타깃팅할 XDM 필드 검색 | 이름, 설명 또는 데이터 값으로 필드를 검색합니다. 해당 필드가 있는 위치와 이미 사용 중인 위치를 확인하세요. | `field-discovery` | Real-Time CDP(RTCDP) | &quot;충성도 고객을 타깃팅하는 데 사용할 수 있는 필드는 무엇입니까?&quot; · &quot;구매 내역과 관련된 필드 찾기&quot; |
| 대상자 게시/저장 | 이름 지정 규칙 및 준수 확인을 사용하여 Experience Platform 세그멘테이션 서비스에 대상 정의 유지 | `audience-publish` | Real-Time CDP(RTCDP) | &quot;초안으로 저장&quot; · &quot;봄 판매 구매자&quot; 이름으로 대상자 게시&quot; |

## 여정

| 사용 사례 | 설명 | 스킬 | 애플리케이션 | 샘플 프롬프트 |
| --- | --- | --- | --- | --- |
| [자연어에서 여정 만들기](journeys/create-journey-from-natural-language.md) | 텍스트 프롬프트 또는 업로드된 이미지/흐름도에서 AJO의 여정 생성 오케스트레이션 | `journey-create` | Adobe Journey Optimizer (AJO) | &quot;등록 후 이메일을 보내고 3일을 기다린 후 후속 작업을 보내는 시작 여정 만들기&quot; · &quot;이 업로드된 순서도 이미지에서 여정 작성&quot; |
| 여정 충돌 분석 | 활성 여정 간 대상 중복 감지, 충돌 예약 및 중복 제거 문제 | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | &quot;장바구니 포기 여정이 다른 여정과 충돌합니까?&quot; · &quot;내 활성 여정 간 대상 겹침 확인&quot; |
| 여정 폴아웃 분석 | 여정 중 고객이 중단되는 위치와 이유를 파악하고, 이탈로 이어지는 행동 패턴을 감지합니다 | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | &quot;내 재참여 여정에서 사람들이 어디에 드롭하고 있습니까?&quot; · &quot;여정 X에서 폴아웃이 가장 높은 노드를 선택하십시오.&quot; |
| 사용자 지정 작업 오류 분석 | 사용자 지정 작업이 실패하거나 여정 내에서 오류율이 급증하는 시점을 식별하고 실패가 더 광범위한 중단으로 이어지기 전에 근본 원인을 진단합니다 | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | &quot;충성도 등록 여정에서 사용자 지정 작업이 실패한 이유는 무엇입니까?&quot; · &quot;시작 여정에서 사용자 지정 작업 ExternalPush에 대한 오류율을 표시합니다.&quot; |
| [충성도 문제를 만들고, 편집하고, 관리합니다](journeys/create-loyalty-challenge.md) | 충성도 프로그램 관리 간소화 및 가속화 | `loyalty` | Adobe Journey Optimizer (AJO) | &quot;회원들이 새로운 계절 음료를 시도하도록 격려하는 도전을 만드세요&quot; · &quot;가장 높은 회원 감소율로 충성도 도전을 보여줍니다.&quot; |

## 기본 요소

| 사용 사례 | 설명 | 스킬 | 애플리케이션 | 샘플 프롬프트 |
| --- | --- | --- | --- | --- |
| 제품 지식 및 설명서 | 공식 Adobe 문서에서 방법, 개념, 문제 해결 및 모범 사례 질문에 답변합니다 | `product-knowledge` | 모든 적격 지원 | &quot;스트리밍 대상을 설정하려면 어떻게 해야 합니까?&quot; · &quot;일괄 처리와 스트리밍 세분화 간의 차이점은 무엇입니까?&quot; |
| Experience Platform/Journey Optimizer 엔티티 쿼리 | 플랫폼 엔터티에 대한 질문을 위한 기본 진입점 역할을 합니다. 필요에 따라 KG, 필드 검색 또는 API로 라우팅합니다. | `operational-insights` | 모든 적격 지원 | &quot;보유한 데이터 세트가 몇 개입니까?&quot; · &quot;모든 활성 여정 표시&quot; · &quot;대상 나열&quot; |
| 지식 그래프 쿼리 | 단일 SQL 쿼리를 통한 집계 카운트, 교차 엔티티 조인, 관계 조회 및 메타데이터 탐색 | `knowledge-graph` | 모든 적격 지원 | &quot;어느 대상자가 이 데이터 세트를 사용합니까?&quot; · &quot;스키마와 데이터 세트 간의 관계 표시&quot; |
| Experience Platform / Journey Optimizer / Customer Journey Analytics API 작업 | 지식 그래프에 없는 돌연변이, 실시간 상태 확인 및 엔티티 유형에 대한 직접 API 게이트웨이 제공 | `cxo-api` | 모든 적격 지원 | &quot;데이터 세트 삭제 X&quot; · &quot;내 일괄 처리 수집 작업의 상태 확인&quot; |
| 엔티티 해결 및 연결 | 의미 체계 및 어휘 검색을 사용하여 실제 Experience Platform 엔티티에 대한 엔티티 언급을 해결하고 XDM 필드를 검색할 수 있습니다 | `entity-linking` | Adobe Experience Platform | &quot;실제 대상자로 &#39;휴일 쇼핑객&#39; 해결&quot; · &quot;구매 내역과 관련된 필드 찾기&quot; |
| 사용자 정의 스킬 관리 | 세션 간에 지속되는 사용자 소유 재사용 가능한 스킬 저장, 수정 또는 삭제 | `manage-skill` | 모든 적격 지원 | &quot;해당 워크플로우를 스킬로 저장&quot; · &quot;내 주간 보고서 스킬 삭제&quot; · &quot;재사용 가능한 스킬로 전환&quot; |

## 샌드박스 도구

| 사용 사례 | 설명 | 스킬 | 애플리케이션 | 샘플 프롬프트 |
| --- | --- | --- | --- | --- |
| [샌드박스 간 개체 이동](/help/agents/sandbox-tooling.md) | 종속성 자동 해결을 통해 샌드박스 간에 스키마, 대상 및 기타 오브젝트 구성을 원활하게 마이그레이션할 수 있습니다. | `sandbox-tooling-workflow` | Adobe Experience Platform | &quot;스키마 Luma 충성도 멤버 플래티넘을 현재 샌드박스에서 프로덕션 샌드박스로 이동&quot; · &quot;미국 Gold 충성도 멤버 대상을 단계로 승격&quot; |
