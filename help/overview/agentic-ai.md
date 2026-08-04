---
title: CX 엔터프라이즈 애플리케이션의 Agentic AI
description: CX Enterprise 애플리케이션에서 AI 에이전트를 사용할 수 있는 위치를 알아봅니다.
solution: Experience Cloud
landing-page-name: ai
landing-page-breadcrumb-title: AI Documentation
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
last-update: '2026-05-21T00:00:00.000Z'
exl-id: c1a8f9a7-4752-4040-b5f0-dc775417f536
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
source-git-commit: a70c6440159ccb7c7544008da5707b23c42468cb
workflow-type: tm+mt
source-wordcount: 1142
ht-degree: 12%

---

# Adobe CX Enterprise의 Agentic AI

Adobe [Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/ko/docs/cx-enterprise-ai/experience-cloud-ai/home)은(는) CX 엔터프라이즈 애플리케이션에서 Agentic AI 기능을 지원합니다.

에이전트는 작업을 자동화하고 통찰력을 신속하게 제공하며 워크플로를 간소화합니다. 따라서 CX Enterprise에서 보다 효율적으로 작업하고 더 많은 가치를 얻을 수 있습니다.

CX Enterprise AI 에이전트는 다음 중 하나에서 사용할 수 있습니다.

* [기존 CX 엔터프라이즈 애플리케이션](#existing-apps)
* [AI 최초 CX 엔터프라이즈 애플리케이션](#ai-first-apps)

다음 섹션에서는 CX Enterprise에서 Agentic AI를 활성화하는 두 가지 방법을 설명합니다.

## 기존 CX 엔터프라이즈 애플리케이션 {#existing-apps}

기존 응용 프로그램에서는 자연어를 사용하여 [AI Assistant](https://experienceleague.adobe.com/ko/docs/cx-enterprise-ai/experience-cloud-ai/home)의 대화 인터페이스를 통해 Adobe Experience Platform 에이전트를 지시할 수 있습니다. AI Assistant는 전체 화면 및 오른쪽 레일 보기에서 모두 사용할 수 있습니다.

에이전트는 다음 범주 중 하나에 해당하는 고객을 위한 기존 CX 엔터프라이즈 앱에서 활성화할 수 있습니다.

* Adobe Experience Platform Agents AI Credits 라이선스를 구입했습니다
* 사용 제한 평가판(제공된 제한된 AI 크레딧)에 포함됩니다
* Agent Orchestrator Promo SKU(시간 제한 체험판 라이선스)를 거래했습니다.

AI 에이전트를 사용하여 _에이전트 작업_&#x200B;을 수행하면 AI 크레딧이 사용됩니다. _[에이전트 작업 및 AI 크레딧 사용](ai-credit-consumption.md)_&#x200B;에서 에이전트 작업 및 AI 크레딧에 대해 자세히 알아보세요.

AI 에이전트는 _귀하의_ 입력 및 감독을 따르며 제품 수준의 액세스 제어를 준수합니다. 기본 CX 엔터프라이즈 애플리케이션에서 사용할 수 있는 권한이 있는 작업이나 데이터에 액세스할 수만 있습니다.

### 기존 CX 엔터프라이즈 앱의 AI 에이전트 {#existing-apps-table}

다음 표에는 기존 CX 엔터프라이즈 애플리케이션에서 사용할 수 있는 Experience Platform Agent 가 나와 있습니다.

| 에이전트 이름 | 기능 | 지원되는 애플리케이션 | 상태 데이터/HIPAA 지원 |
|---|----------|----------|----------|
| [Audience Agent](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/agents/audience) | 자연어 프롬프트를 통해 보다 쉽고, 효율적이며, 시장 출시 속도를 높여 고객을 관리하고 최적화할 수 있습니다. | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | |
| [콘텐츠 어드바이저 에이전트](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/content-advisor/overview) | <ul><li>자연어를 사용하여 팀이 기업 전체에서 가장 관련성이 높은 컨텐츠를 신속하게 찾을 수 있도록 지원하므로 검색 시간이 단축되고 의사 결정 및 실행 속도가 빨라집니다.</li><li>자연어 프롬프트를 사용하여 소스 에셋에서 시각적 콘텐츠 변형을 쉽게 만들 수 있습니다.</li></ul> | <ul><li>Adobe Experience Manager Assets</li></ul><ul><li>Dynamic Media(클라우드 서비스)</li></ul> | |
| [Data Insights Agent](https://experienceleague.adobe.com/ko/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) | 데이터에 대한 질문에 신속하게 답변할 수 있습니다. 데이터 보기의 구성 요소와 실제 데이터를 사용하여 Analysis Workspace에서 관련 시각화를 빌드합니다. | <ul><li>Customer Journey Analytics (B2B 및 B2C 에디션)</li></ul> | 예 |
| [브랜드 경험 에이전트](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/brand-experience/overview) | <ul><li>기존 사이트를 자동으로 재구성, 강화 및 검증하여 디지털 경험의 마이그레이션 및 현대화 속도를 높임으로써 팀이 위험과 수작업을 줄이면서 최신 AI 지원 경험으로 빠르게 이동할 수 있습니다.</li><li>대규모 환경 생성 및 업데이트를 통해 수작업과 주기 시간을 대폭 단축하여 품질이나 일관성을 유지하면서 팀을 더욱 빠르게 이동시킬 수 있습니다.</li><li>양식 경험을 자동으로 생성, 구성 및 검증하여 최적화된 온브랜드 양식을 신속하게 만들 수 있으므로 팀이 최소한의 수작업으로 더 높은 품질의 데이터를 빠르게 시작하고 캡처할 수 있습니다.</li><li>AEM CS 개발자와 기술 관리자가 근본 원인을 분석하고 수정 사항을 제시하여 Cloud Manager 파이프라인의 빌드 단계 오류를 해결할 수 있도록 지원합니다.</li></ul> | <ul><li>Adobe Experience Manager Sites Cloud Services(Experience 현대화)</li></ul><ul><li>Adobe Experience Manager Sites(Experience Production)</li></ul><ul><li>Adobe Experience Manager Forms(양식 만들기)</li></ul><ul><li>모든 클라우드 기반 Adobe Experience Manager 애플리케이션(개발 지원)</li></ul> | |
| [브랜드 거버넌스 에이전트](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/governance/overview) | 실시간 거버넌스로 DRM을 지원하기 위해 자동화된 브랜드 정책 확인, 권한 및 인텔리전스를 통해 브랜드 무결성 및 규정 준수를 보호합니다. | <ul><li>Adobe Experience Manager Assets</li><li>Adobe Experience Manager Sites(브랜드 정책)</li></ul> | |
| [Journey Agent](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/ajo-agent) | 팀이 규모에 맞게 멀티 터치 고객 여정을 신속하게 분석하고 최적화할 수 있습니다. | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | |
| [제품 지원 에이전트](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/product-support) | 워크플로우를 종료하지 않고 지원 문제를 해결하고, 고객 지원 티켓을 만들고, AI Assistant를 사용하여 사례 진행 상황을 추적합니다. | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li><li>Customer Journey Analytics (B2B 및 B2C 에디션)</li><li>Adobe Experience Manager</li></ul> | |
| [Adobe Marketing Agent for Microsoft 365 Copilot](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/agents/ama-ms) | Experience Platform을 Microsoft 365 Copilot에 직접 연결합니다. Teams, Word, Powerpoint 및 Excel과 같은 Microsoft 365 애플리케이션 내에서 자연어 질문을 하면 워크플로를 중단하지 않고 Experience Platform에서 마케팅 인사이트를 즉시 검색할 수 있습니다. | <ul><li> Audience Agent, Journey Agent, Customer Journey Analytics Data Insights, Experience Platform Operational Insights를 지원하는 Adobe Agent Orchestrator</li></ul> | |

## AI 최초 CX 엔터프라이즈 애플리케이션 {#ai-first-apps}

AI 우선 애플리케이션은 생성 또는 아젠틱 AI를 주요 구성 요소로 하여 구축됩니다. 이들은 핵심 업무에 생성 또는 agentic AI를 사용하며, 아젠틱 기능은 이미 AI 우선 애플리케이션 라이선스에 포함되어 있다. 따라서 Experience Platform Agent Orchestrator 라이선스가 필요하지 않습니다.

다음 표에는 AI 우선 애플리케이션으로 사용할 수 있는 Experience Platform 에이전트가 나열되어 있습니다. 이러한 AI 기반 애플리케이션은 다음과 같은 라이센스를 통해 사용할 수 있습니다.

| 에이전트 이름 | 기능 | 지원되는 애플리케이션 |
|---|----------|----------|
| [Experimentation Agent](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/content-experiment/experiment/experiment-accelerator-security) | 인사이트를 자동화, 분석 및 합성하므로 수작업 프로세스를 줄이면서 중앙 집중식 작업 공간에서 영향력이 큰 실험 및 성장 기회를 신속하게 식별할 수 있습니다. | <ul><li>AJO Experimentation Accelerator</li></ul> |
| [LLM 최적화 에이전트](https://experienceleague.adobe.com/ko/docs/llm-optimizer/using/home) | AI 기반 검색 환경에서 가시성, 정확성 및 영향력을 강화하고, AI가 생성한 답변의 브랜드 존재감에 대한 통찰력을 제공하고, 규범적인 콘텐츠 권장 사항을 제공하고, 최적화 수정 사항을 자동화합니다. | <ul><li>Adobe LLM Optimizer</li></ul> |
| [Site Optimization Agent](https://experienceleague.adobe.com/ko/docs/experience-manager-sites-optimizer/content/home) | 향상된 웹 사이트를 자동으로 감지하고 배포하여 비즈니스 효과를 극대화합니다. 생성 AI와 여러 모니터링 기술을 사용하면 사이트 트래픽 획득, 참여 등을 향상시킬 수 있습니다 | <ul><li>AEM Sites Optimizer</li></ul> |
| [Product Advisor Agent](https://experienceleague.adobe.com/en/docs/brand-concierge/content/documentation/overview) | 개별 환경 설정 및 행동에 맞게 맞춤화된 지능적인 컨텍스트 인식 제품 검색을 통해 전환과 참여를 강화할 수 있습니다. | <ul><li>Adobe Brand Concierge</li></ul> |

## 이 항목에 대한 추가 도움말

* [CX 엔터프라이즈 에이전트 툴](https://experienceleague.adobe.com/en/docs/cx-enterprise-agentic-tools/using/overview#adobe-cx-enterprise-agentic-tools)
* [에이전트 작업 및 AI 신용 소비](ai-credit-consumption.md)
* CX Enterprise의 [AI](https://experienceleague.adobe.com/ko/docs/ai) 설명서 홈
* [AEM의 에이전트 개요](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/overview)

[!BADGE Adobe for Business에 대해 자세히 알아보기]{type=Informative url="https://business.adobe.com/products/experience-platform/agent-orchestrator.html" tooltip="Business.adobe.com으로 이동"}
