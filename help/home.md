---
title: CX Enterprise 애플리케이션의 AI
description: CX 엔터프라이즈 애플리케이션이 생성 AI(GenAI), AI Assistant, Agentic AI, CX Enterprise Coworker 및 MCP 도구를 사용하는 방법을 알아봅니다.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: e15ac0578299c0dbc029f178fa028652cc5bb462
workflow-type: tm+mt
source-wordcount: 873
ht-degree: 4%

---

# CX Enterprise의 AI

이 안내서에서는 Adobe CX Enterprise의 AI 기능인 생성 AI, AI Assistant, Agent Orchestrator, Experience Platform Agents, CX Enterprise Coworker 및 MCP를 다룹니다.

## AI 기능 개요

여기에서 CX Enterprise에서 AI를 사용하는 위치와 방법에 대한 입문서를 시작하십시오.

- [생성 AI](./overview/generative-ai.md)은(는) 생성 AI 및 AI Assistant를 지원하는 CX 엔터프라이즈 애플리케이션과 비교 방법을 설명합니다.
- [Agentic AI](./overview/agentic-ai.md)에서는 Experience Platform 에이전트가 기존 CX 엔터프라이즈 응용 프로그램과 AI 우선 응용 프로그램 모두에서 작동하는 방식을 설명하고 각 응용 프로그램에서 사용할 수 있는 에이전트를 나열합니다.
- [Agentic AI 모니터링](./overview/monitoring.md)은(는) 에이전트 채택, 사용, 피드백 및 AI 크레딧 소비를 추적하는 대시보드를 다룹니다.
- [에이전트 작업 및 AI 크레딧 사용](./overview/ai-credit-consumption.md)에서는 에이전트 작업과 작업 유형별로 예상 소비율을 사용하여 에이전트 작업이 AI 크레딧을 사용하는 방법을 설명합니다.
- [CX 엔터프라이즈 에이전트 도구](https://experienceleague.adobe.com/ko/docs/cx-enterprise-agentic-tools/using/overview)에서는 CX 엔터프라이즈 에이전트를 확장하는 추가 에이전트 기술 및 도구를 다룹니다(비디오 튜토리얼).

## AI 어시스턴트

[AI Assistant](./ai-assistant/ai-assistant-ui.md)은(는) Adobe Experience Platform 기반 애플리케이션에서 사용할 수 있는 대화식 생성 AI 도구입니다. 전체 화면 또는 레일 보기 인터페이스에서 자연어 프롬프트를 통해 제품 지식을 얻고 문제를 해결하며 운영 통찰력을 찾고 Experience Platform 에이전트에 액세스할 수 있습니다.

인터페이스를 탐색하는 방법을 알아보려면 [AI Assistant UI 안내서](./ai-assistant/ai-assistant-ui.md)를 읽어 보십시오. 에이전트별 예제 프롬프트를 보려면 [프롬프트 라이브러리](./ai-assistant/prompt-library.md)를 참조하십시오.

## Agent Orchestrator 및 Experience Platform 에이전트

[Agent Orchestrator](./agents/agent-orchestrator.md)은(는) Experience Platform 에이전트를 구동하는 에이전트 계층입니다. AI 어시스턴트에게 질문을 하면 Agent Orchestrator이 작업을 계획하고 이에 답변하는 데 필요한 전문 에이전트를 호출한 후 통합된 응답을 반환합니다(모두 사람 감독).

이 안내서에는 다음 Experience Platform 에이전트가 설명되어 있습니다.

- [Audience 에이전트](./agents/audience.md)
- [Data Insights Agent](./agents/cja-data-insights-agent.md)
- [Experimentation Agent](./agents/agent-experiment.md)
- [필드 검색 에이전트](./agents/field-discovery-agent.md)
- [Journey Agent](./agents/ajo-agent.md)
- [알림 에이전트](./agents/notifications.md)
- [제품 지원 에이전트](./agents/product-support.md)
- [Adobe Marketing Agent for Microsoft 365 Copilot](./agents/ama-ms.md)
- [데이터 유효성 검사](./agents/data-validation.md)

에이전트, 각 에이전트가 지원하는 애플리케이션 및 자격 요구 사항에 대한 전체 목록은 [CX Enterprise의 Agentic AI](./overview/agentic-ai.md)를 참조하십시오.

## CX Enterprise Coworker

CX Enterprise Coworker는 고객 경험 및 마케팅 워크플로우를 자동화하는 에이전트 중심의 AI Assistant로 일상적인 실행 대신 비즈니스 목표에 집중할 수 있도록 지원합니다. 한 번에 한 질문씩 던지는 대신 목표를 설명한다. 동료는 사용자의 승인을 위해 완료된 작업을 계획, 실행, 검증 및 반환합니다. 동료는 다음과 같습니다.

- **[공동 작업자 채팅](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/overview)**: 데이터를 탐색하고, 대상자와 여정의 유효성을 검사하고, CX 엔터프라이즈 애플리케이션에서 여러 단계 작업을 완료할 수 있는 대화형 인터페이스입니다.
- **[공동 작업자 캠페인](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/overview)**: 캠페인 브리핑, 대상자 작성, 콘텐츠 생성, 여정 디자인 및 증명을 하나의 대화 경험으로 통합하는 AI 기반 애플리케이션입니다. 내장된 템플릿, 모범 사례 및 안내 메시지를 활용하여 민첩한 소규모 팀이 신속하게 캠페인을 시작할 수 있도록 지원합니다.
- **공동 작업자 프로젝트**(준비 중): 엔드 투 엔드 고객 경험 오케스트레이션 워크플로우를 자동화하고, 팀이 작업, 승인 및 실행을 조정하여 전략에서 게재를 통한 결과를 도출하는 데 도움이 되는 통합 작업 영역입니다. 프로젝트 설명서가 곧 제공됩니다.

적격 고객이 점차 AI 비서 및 Experience Platform 에이전트에서 동료채팅으로 전환되고 있습니다. 평가판 자격, AI 크레딧 사용 방법 및 액세스 방법에 대해 알아보려면 [CX Enterprise Coworker 평가판](./agents/trial.md)을 읽어 보십시오.

동료 채팅을 실제로 보려면 [플레이그라운드에서 동료 채팅](./coworker/playground-coworker-chat.md)을 살펴보거나 [CJA 마이그레이션 데이터에 대한 AA 유효성 검사](./coworker/data-validation-aa-cja.md) 및 [CJA 데이터 분석](./coworker/chat/analytics-chat.md)과 같은 실제 사용 사례를 읽어 보십시오.

동료 채팅, 캠페인 및 프로젝트에 대한 전체 제품 설명서는 [Adobe CX Enterprise Coworker](./coworker/overview.md)를 참조하십시오. 샌드박스 간 개체 복제에 대해서는 [샌드박스 도구 에이전트 기술](./agents/sandbox-tooling.md)을 참조하십시오.

## MCP

[Adobe CX Coworker Gateway](./mcp/overview.md)은(는) CX Enterprise용 MCP(Unified Model Context Protocol) 종단점입니다. [!DNL Claude], [!DNL ChatGPT] 및 [!DNL Cursor]과(와) 같은 MCP 호환 클라이언트에게 조직이 사용할 수 있는 제품 도구에 대한 단일 관리 연결을 제공합니다. 이러한 도구에는 [!DNL Real-Time CDP], [!DNL Experience Platform], [!DNL Journey Optimizer], [!DNL Customer Journey Analytics], [!DNL Adobe Analytics] 및 [!DNL Workfront]이(가) 포함됩니다.

CX Coworker Gateway를 처음 사용하십니까? 연결하려면 [CX Coworker Gateway 도구 액세스](./mcp/access.md) 및 [CX Coworker Gateway 설치](./mcp/install.md)를 참조하십시오.

## 시작하기

### 액세스 요구 사항

AI Assistant 및 Experience Platform 에이전트를 사용하려면 Adobe 관리자가 적절한 권한을 부여해야 합니다. 요구 사항은 애플리케이션에 따라 다릅니다. 자세한 내용은 Agent Orchestrator 안내서의 [액세스](./agents/agent-orchestrator.md#access)를 참조하십시오.

### 개인정보보호 및 보안

AI Assistant 및 Experience Platform 에이전트는 샌드박스별 데이터 격리와 기존 액세스 제어 정책을 포함하여 개인 정보, 보안 및 거버넌스의 우선순위를 지정합니다. 자세한 내용은 [AI Assistant의 개인 정보, 보안 및 거버넌스](./ai-assistant/privacy.md)를 참조하십시오.

## 모범 사례

AI Assistant 또는 동료 경험을 통해 최대의 가치를 얻으려면 다음 모범 사례를 따르십시오.

- 대상 및 관련 인사이트를 얻으려면 프롬프트에 **구체적으로**&#x200B;하십시오.
- 제공된 원본 인용과 추론 설명을 검토하여 **응답을 확인**&#x200B;합니다.
- **컨텍스트 설정을 사용**&#x200B;하여 가장 관련성이 높은 데이터 원본이 질문에 사용되었는지 확인하세요.
- **피드백을 제공**&#x200B;하여 시간이 지남에 따라 성능과 정확도를 개선하십시오.
- 보다 포괄적인 분석을 위해 여러 에이전트의 **통찰력을 결합**.

## 법적 고려 사항

AI 어시스턴트는 현재 영어로만 응답을 지원하고 있으며, 언어 모델이 가끔 실수를 하기도 한다. 제공된 정보를 항상 확인하고 각 응답에 포함된 추론 단계를 사용하여 생성 방법을 이해합니다. 자세한 내용은 [법적 고지 사항](./ai-assistant/legal-disclaimer.md)을 참조하세요.

