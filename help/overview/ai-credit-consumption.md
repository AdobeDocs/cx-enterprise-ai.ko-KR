---
title: 에이전트 작업 및 AI 크레딧 사용량
description: CX Enterprise 애플리케이션의 에이전트 작업 및 AI 크레딧 사용률에 대해 알아봅니다.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
last-update: '2026-05-21T00:00:00.000Z'
source-git-commit: cbded236e67d7d47ad70187a307f403a93ace8e9
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 8%

---

# Adobe Experience Platform 에이전트 작업 및 AI 크레딧 소비

CX 엔터프라이즈 애플리케이션의 에이전트 AI 작업 및 AI 크레딧 사용량에 대해 알아봅니다. 기존 CX 엔터프라이즈 애플리케이션에서 Agentic AI 기능을 활성화하는 방법에 대한 자세한 내용은 [CX Enterprise의 Agentic AI](agentic-ai.md#existing-apps)를 참조하십시오.

## 새로운 기능

| 기능 | 설명 |
| --- | --- |
| [CX 엔터프라이즈 에이전트 AI 기능 카탈로그](https://agentic-capability-explorer.entapp.adproto.com/) | 라이선스가 부여된 CX Enterprise 앱에서 사용할 수 있는 에이전틱 AI 작업을 알아보십시오. |

## 에이전트 작업

_에이전트 작업_&#x200B;은(는) 고객 입력의 지시에 따라 특정 결과를 얻기 위해 에이전트가 실행하는 일련의 작업 및 작업입니다.

AI Assistant를 통해 자연어 프롬프트를 사용하면 에이전트에게 특정 작업을 수행하도록 요청할 수 있습니다. 이러한 정보를 바탕으로 Agent Orchestrator은 관련 CX 엔터프라이즈 애플리케이션에서 각 단계를 실행하도록 적절한 에이전트를 조정합니다.

## AI 크레딧

_AI 크레딧_&#x200B;은 에이전트 작업의 실행을 수량화하는 사용 기반 지표입니다. AI 크레딧이 [AI 우선 애플리케이션](agentic-ai.md)에 적용되지 않습니다.

## AI 신용 소비

AI 크레딧 사용은 실행된 작업의 복잡성과 가치에 따라 달라질 수 있습니다.

* 간단한(종종 단일 단계) 작업은 더 적은 크레딧을 사용합니다
* 복잡한(종종 여러 단계) 작업이 더 많은 크레딧을 소비함
* 고급 추론, 유효성 검사, 다중 에이전트 조정 또는 통합과 관련된 작업은 더 많은 크레딧을 사용합니다.

**참고:** [CX Enterprise Agentic AI 기능 카탈로그](https://agentic-capability-explorer.entapp.adproto.com/)를 사용하여 라이선스가 부여된 CX Enterprise 앱에서 사용 가능한 Agentic AI 작업을 확인할 수도 있습니다.

### 예상 AI 크레딧 소비율

| 에이전트 | 작업 | 지원되는 애플리케이션 | 예상 AI 점수 | 샘플 프롬프트 |
| ------ | ----- | ------------------------ | ----------------------- | ----------------- |
| Audience 에이전트 | 대상자/계정 관념화 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 50 | <ul><li><em>부유한 구매자를 위한 필드 표시</em></li><li><em>고객 환경 설정과 관련된 모든 필드 찾기</em></li></ul> |
| Audience 에이전트 | 대상자 / 계정 관리 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 25 | <ul><li><em>중복 대상이 있습니까?</em></li><li><em>가장 큰 대상자 5명을 표시합니다.</em></li><li><em>대상에 대해 활성화되지 않은 대상 표시</em></li><li><em>라이브 여정에 사용된 모든 대상 나열</em></li></ul> |
| Audience 에이전트 | 대상자/계정 분석 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 25 | <ul><li><em>지난 주에 20% 이상 증가한 대상은 무엇입니까?</em></li><li><em>30일 전 값과 비교하여 대상 &quot;단골 플래티넘&quot;이 얼마나 변경되었습니까?</em></li><li><em>가장 빠르게 성장하는 대상자는 무엇입니까?</em></li></ul> |
| Audience 에이전트 | 구매 그룹 관념화 | <ul><li>Adobe Journey Optimizer(B2B edition)</li></ul> | 25 | <ul><li><em>이 제품에 대한 의도를 표시하는 계정은 무엇입니까?</em></li><li><em>XYZ의 제품 의도로 최상위 사용자를 보여 주십시오.</em></li><li><em>5명 이상의 회원이 있는 구매 그룹</em></li></ul> |
| Data Insights Agent | 데이터 분석 및 시각화 | <ul><li>Customer Journey Analytics (B2C 및 B2B 에디션)</li></ul> | 25 | <ul><li><em>7월 주문 트렌드</em></li><li><em>지역별 매출을 표시합니다.</em></li><li><em>3월부터 6월까지 성별 주문 표시</em></li><li><em>6월 수익별 상위 10개 SKU는 무엇입니까</em></li><li><em>연간 월별 구매 비율</em></li><li><em>제품 범주별 매출 점유율</em></li></ul> |
| Journey Agent | 여정 관념화 | <ul><li>Adobe Journey Optimizer(B2B edition)</li></ul> | 25 | <ul><li><em>웹 사이트에서 콘텐츠에 관여하는 사람들에게 초점을 맞추어 내 솔루션을 위한 여정을 만들어 스페이스 계정을 만드세요</em></li></ul> |
| Journey Agent | 여정 분석 | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | 50 | <ul><li><em>7월 4일 여정에 대한 노드별 폴아웃을 분석하려고 합니다.</em></li><li><em>여정 X에 대해 일정 충돌이 있습니까</em></li><li><em>여정 X에 대한 대상 겹침 표시</em></li></ul> |
| Journey Agent | 여정 관리 | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | 25 | <ul><li><em>라이브 여정이 몇 개나 있습니까?</em></li><li><em>대상 X를 사용하여 모든 여정 나열.</em></li><li><em>현재 테스트 모드에 있는 모든 여정 나열</em></li></ul> |
| 제품 지원 에이전트 | 지식 기반 문제 해결 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer (B2C 및 B2B 에디션)</li><li>Customer Journey Analytics (B2C 및 B2B 에디션)</li></ul> | 0 | <ul><li><em>라이선스 사용 대시보드와 Experience Platform 홈 페이지에서 프로필 수가 다른 이유는 무엇입니까?</em></li><li><em>여정이 트리거되지 않는 이유는 무엇입니까?</em></li><li><em>Adobe Experience Platform에서 실시간 경험을 만드는 방법은 무엇입니까?</em></li><li><em>Adobe Experience Platform에서 경고를 구성하고 사용하는 방법은 무엇입니까?</em></li><li><em>Adobe Experience Platform 활성화의 평균 프로필 풍부도 제한은 얼마입니까?</em></li></ul> |
| 제품 지원 에이전트 | 지원 사례 만들기 및 추적 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer (B2C 및 B2B 에디션)</li><li>Customer Journey Analytics (B2C 및 B2B 에디션)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li><em>실패한 세분화 작업에 대한 새 지원 티켓 만들기</em></li><li><em>티켓 전자 메일의 001772068이 무엇입니까?</em></li></ul> |
| 콘텐츠 관리자 에이전트 | 콘텐츠 검색 | <ul><li>Adobe Experience Manager</li></ul> | 5 | <ul><li><em>WKND 오퍼 캠페인을 만들기 위한 콘텐츠 조각을 표시합니다.</em></li><li><em>제품 패키지 PNG 이미지를 찾습니다.</em></li><li><em>WKND 폴더에 태그가 지정된 Office 이미지를 표시합니다.</em></li><li><em>WKND 폴더에 svgs가 있습니까?</em></li><li><em>대출 신청서 양식을 모두 표시합니다.</em></li><li><em>직원 온보딩 양식을 찾고 있습니다.</em></li></ul> |
| 콘텐츠 관리자 에이전트 | <ul><li>콘텐츠 최적화</li></ul> | <ul><li>Adobe Experience Manager Assets 및 Dynamic Media</li></ul> | 10 | <ul><li><em>2000px 렌디션을 JPEG으로 80% 품질로 만듭니다.</em></li><li><em>Instagram 스토리에 대한 렌디션을 만듭니다.</em></li><li><em>이미지 위에 30% 할인 그래픽으로 이미지를 오버레이하여 중앙에서 100px를 배치합니다.</em></li><li><em>PNG의 배경색을 #ff8932.</em></li></ul> |
| 브랜드 거버넌스 에이전트 | <ul><li>브랜드 정책 확인</li></ul><ul><li>Content Hub을 사용한 권한</li></ul><ul><li>에셋 만료</li></ul> | <ul><li>Adobe Experience Manager Sites(브랜드 정책)</li></ul><ul><li>Adobe Experience Manager Assets</li></ul> | 25 | <ul><li><em>이 페이지가 내 브랜드와 일치합니까? `https://www.website/en.html`</em></li><li><em>기존 Content Hub ABAC 규칙 모두 표시</em></li><li><em>내 자산이 곧 만료됩니까?</em></li></ul> |
| Brand Experience Agent | <ul><li>콘텐츠 업데이트</li><li>Forms 제작</li><li>파이프라인 문제 해결</li></ul> | <ul><li>Adobe Experience Manager 클라우드 서비스</li><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Forms</li></ul> | 50 | <ul><li><em>`URL`에 헤드라인을 Hello World로 업데이트</em></li><li><em>이름, 전자 메일 및 메시지 필드가 있는 연락처 양식을 만듭니다</em></li><li><em>실패한 파이프라인 문제 해결</em></li><li><em>주 프로그램에 대해 실패한 파이프라인을 나열합니다.</em></li></ul> |
| Brand Experience Agent | 사이트 현대화 | Adobe Experience Manager 클라우드 서비스 | 100 | <ul><li><em>페이지 `https://wknd-trendsetters.site`</em> 마이그레이션</li></ul> |

>[!NOTE]
>
>실제 AI 크레딧 소비는 실행된 단계 수와 단계당 반복 횟수에 따라 달라질 수 있습니다.

## 이 항목에 대한 추가 도움말

* [CX Enterprise의 GenAI](generative-ai.md)
* [CX Enterprise의 에이전트 AI](agentic-ai.md)
* [Adobe Experience Platform Agents 사용 바인딩된 체험판](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)
