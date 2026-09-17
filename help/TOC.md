---
audience: user
user-guide-title: CX Enterprise의 AI
user-guide-description: 실용적인 설명서, 구현 지침 및 참조 자료를 통해 AI Assistant, Coworker, 에이전트 및 MCP를 구축, 구성, 통합 및 확장하는 방법을 알아봅니다.
description: CX Enterprise의 AI 도구에 대해 알아봅니다. CX Enterprise에서 AI를 사용하여 제품 지식을 향상시키고 운영 통찰력을 얻으십시오.
solution: Experience Cloud
role: Admin,User,Developer,Leader
dummy: true
source-git-commit: 1f9534bea8653a8dcf4dc89f5f7f2702477b6c97
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 18%
---

# CX Enterprise의 AI {#experience-cloud-ai}

- [CX Enterprise의 AI](home.md)
- CX Enterprise의 AI 정보 {#overview}
  - [CX Enterprise의 AI 정보](./overview/overview-ai-cxe.md)
  - [생성 AI 정보](./overview/generative-ai.md)
  - [아젠틱 AI 정보](./overview/agentic-ai.md)
  - [AI 크레딧 소비 정보](./overview/ai-credit-consumption.md)
  - [Agentic AI 모니터링 대시보드](./overview/monitoring.md)
  - [에이전틱 도구](https://experienceleague.adobe.com/ko/docs/cx-enterprise-agentic-tools/using/overview)
  - [생성 AI 콘텐츠 투명도](content-transparency.md)
- CX Enterprise Coworker {#coworker}
  - [동료 기본 정보](./coworker/overview.md)
  - 채팅 {#chat}
    - [개요](./coworker/chat/overview.md)
    - [UI 안내서](./coworker/chat/ui-guide.md)
    - {hide-from-toc}[플레이그라운드에서 동료 채팅](./coworker/playground-coworker-chat.md)
    - 사용 사례 {#use-cases}
      - [동료 채팅 사용 사례](./coworker/chat/use-cases/overview.md)
      - 데이터 인사이트 {#data-insights}
        - [CJA 데이터 분석](./coworker/chat/use-cases/data-insights/analytics-chat.md)
        - [트렌드 및 근본 원인 탐색](./coworker/chat/use-cases/data-insights/root-cause-analysis.md)
        - [업그레이드 시 AA에서 CJA 데이터로의 유효성 검사](./coworker/chat/use-cases/data-insights/data-validation-aa-cja.md)
        - [CJA 보고를 위한 데이터 세트 품질 유효성 검사](./coworker/chat/use-cases/data-insights/validate-dataset-quality-for-cja.md)
      - 대상자 {#audiences}
        - [플랫폼 상태 평가 및 대상 구축](./coworker/chat/use-cases/audiences/create-audience-from-natural-language.md)
      - 여정 {#journeys}
        - [자연어를 사용하여 여정 만들기](./coworker/chat/use-cases/journeys/create-journey-from-natural-language.md)
      - 충성도 {#loyalty}
        - [충성도 과제 및 잠재 고객 인사이트 만들기](./coworker/chat/use-cases/journeys/create-loyalty-challenge.md)
      - 최적화 {#optimization}
        - [Target 활동 시작](./coworker/chat/use-cases/optimization/target.md)
      - 샌드박스 도구 {#sandbox-tooling}
        - [샌드박스 도구 에이전트 기술](./agents/sandbox-tooling.md)
      - 경고 {#alerts}
        - [고객 경고 기술](./agents/customer-alerts.md)
      - 콘텐츠 관리자 {#content-advisor}
        - [마케팅 에셋 생성](./coworker/chat/use-cases/content-advisor/generate-assets.md)
        - [브랜드 준수 검사](./coworker/chat/use-cases/content-advisor/brand-compliance.md)
  - 사용자 지정 {#customizations}
    - 기술 {#skills}
      - [기술이란?](./coworker/customizations/skills/what-are-skills.md)
      - [첫 번째 스킬 만들기](./coworker/customizations/skills/create-your-first-skill.md)
      - [품질 게이트 스킬 구축 및 실행](./coworker/customizations/skills/run-a-quality-gate-skill.md)
      - [기술 관리 및 반복](./coworker/customizations/skills/manage-and-iterate-on-skills.md)
  - 캠페인 {#campaigns}
    - [개요](./coworker/campaigns/overview.md)
    - [이메일 캠페인 만들기](./coworker/campaigns/create-an-email-campaign.md)
    - [사용 사례](./coworker/campaigns/use-cases.md)
    - [프롬프트 우수 사례](./coworker/campaigns/prompting-best-practices.md)
    - [C2PA 메타데이터](./coworker/campaigns/c2pa-metadata.md)
    - 커넥터 {#connectors}
      - [Marketo Engage](./coworker/campaigns/connectors/marketo.md)
      - [Hubspot](./coworker/campaigns/connectors/hubspot.md)
    - [릴리스 정보](./coworker/campaigns/release-notes.md)
- AI 어시스턴트 {#ai-assistant}
  - [AI Assistant UI 안내서](./ai-assistant/ai-assistant-ui.md)
  - [프롬프트 라이브러리](./ai-assistant/prompt-library.md)
  - [개인 정보 보호](./ai-assistant/privacy.md)
  - [법적 면책 조항](./ai-assistant/legal-disclaimer.md)
- 에이전트 {#agents}
  - [Agent Orchestrator](./agents/agent-orchestrator.md)
  - [Audience 에이전트](./agents/audience.md)
  - [Data Insights Agent](./agents/cja-data-insights-agent.md)
  - [실험 에이전트](./agents/agent-experiment.md)
  - [필드 검색 에이전트](./agents/field-discovery-agent.md)
  - [Journey Agent](./agents/ajo-agent.md)
  - [제품 지원 에이전트](./agents/product-support.md)
  - [Adobe Marketing Agent for Microsoft 365 Copilot](./agents/ama-ms.md)
  - [알림 에이전트](./agents/notifications.md)
  - [동료 시험](./agents/trial.md)
  - [데이터 유효성 검사](./agents/data-validation.md)
  - 데이터 엔지니어링 {#data-engineering}
    - {hide-from-toc}[Data Engineering Agent](./agents/data-engineering/overview.md)
- MCP {#mcp}
  - {hide-from-toc}[Adobe CX Coworker 게이트웨이](./mcp/overview.md)
  - {hide-from-toc}[Real-Time CDP MCP 베타](./mcp/beta/rtcdp-mcp.md)
  - 시작하기 {#mcp-get-started}
    - {hide-from-toc}[CX Coworker 게이트웨이 도구 액세스](./mcp/access.md)
    - {hide-from-toc}[CX Coworker 게이트웨이 설치](./mcp/install.md)
    - {hide-from-toc}[CX Coworker 게이트웨이의 세션 컨텍스트 도구](./mcp/context-tools.md)
  - 제품 도구 {#mcp-product-tools}
    - {hide-from-toc}[Real-Time CDP 도구](./mcp/rtcdp-mcp.md)
    - {hide-from-toc}[Experience Platform 도구](./mcp/aep-mcp.md)
    - {hide-from-toc}[Journey Optimizer 도구](./mcp/ajo-mcp.md)
    - {hide-from-toc}[Customer Journey Analytics 도구](./mcp/cja-mcp.md)
    - {hide-from-toc}[Adobe Analytics 도구](./mcp/analytics-mcp.md)
    - [Workfront](https://experienceleague.adobe.com/en/docs/workfront/using/basics/workfront-mcp-server/workfront-mcp-server-overview)
    - [대상](https://experienceleague.adobe.com/en/docs/target/using/mcp/target-mcp)

