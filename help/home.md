---
title: CX 엔터프라이즈 애플리케이션의 AI
description: CX 엔터프라이즈 애플리케이션이 생성 AI(GenAI), AI Assistant, Agentic AI, CX Enterprise Coworker 및 MCP 도구를 사용하는 방법을 알아봅니다.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: d8daade8bb7d0259cd18fe7c8f957955dd97b2a0
workflow-type: tm+mt
source-wordcount: 766
ht-degree: 2%

---

# CX Enterprise의 AI

이 안내서에서는 Adobe CX Enterprise 애플리케이션에서 사용할 수 있는 AI 기능에 대해 설명합니다. 제품 지식 및 운영 통찰력을 위한 생성 AI 및 AI 지원, 작업을 자동화하는 Agent Orchestrator 및 Experience Platform 에이전트, 완전히 대화하는 에이전트 우선 경험을 위한 CX Enterprise Coworker 및 CX Enterprise 데이터에 고유한 AI 도구를 연결하는 MCP.

## CX Enterprise의 AI 정보

여기에서 CX Enterprise에서 AI를 사용하는 위치와 방법에 대한 입문서를 시작하십시오.

- [생성 AI](./overview/generative-ai.md)은(는) 생성 AI 및 AI Assistant를 지원하는 CX 엔터프라이즈 애플리케이션과 비교 방법을 설명합니다.
- [Agentic AI](./overview/agentic-ai.md)에서는 Experience Platform 에이전트가 기존 CX 엔터프라이즈 응용 프로그램과 AI 우선 응용 프로그램 모두에서 작동하는 방식을 설명하고 각 응용 프로그램에서 사용할 수 있는 에이전트를 나열합니다.
- [Agentic AI 모니터링](./overview/monitoring.md)은(는) 에이전트 채택, 사용, 피드백 및 AI 크레딧 소비를 추적하는 대시보드를 다룹니다.
- [에이전트 작업 및 AI 크레딧 사용량](./overview/ai-credit-consumption.md)에서는 에이전트 작업 및 작업 유형별 예상 소비율과 함께 AI 크레딧이 에이전트 작업에서 사용되는 방식을 설명합니다.

## AI 어시스턴트

[AI Assistant](./ai-assistant/ai-assistant-ui.md)은(는) Adobe Experience Platform 기반 애플리케이션에서 사용할 수 있는 대화식 생성 AI 도구입니다. 전체 화면 또는 레일 보기 인터페이스에서 자연어 프롬프트를 통해 제품 지식을 얻고 문제를 해결하며 운영 통찰력을 찾고 Experience Platform 에이전트에 액세스할 수 있습니다.

인터페이스를 탐색하는 방법을 알아보려면 [AI Assistant UI 안내서](./ai-assistant/ai-assistant-ui.md)를 읽고, 예를 들어 에이전트에서 메시지를 보내는 경우 [프롬프트 라이브러리](./ai-assistant/prompt-library.md)를 읽어 보십시오.

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

에이전트, 각 에이전트가 지원하는 애플리케이션 및 자격 요구 사항에 대한 전체 목록은 [CX Enterprise의 Agentic AI](./overview/agentic-ai.md)를 참조하십시오.

## CX Enterprise Coworker

CX Enterprise Coworker는 AI Assistant의 에이전트 우선 제품입니다. 한 번에 한 질문씩 대답하는 대신 목표를 자연어로 설명하면 Coworker가 작업을 계획하고, Adobe 및 연결된 시스템 전반에서 실행하고, 결과를 검증하고, 완료된 작업을 사용자의 승인을 위해 반환합니다. 동료는 다음과 같습니다.

- **공동 작업자 채팅**: 데이터를 탐색하고, 대상자와 여정의 유효성을 검사하고, CX 엔터프라이즈 애플리케이션에서 여러 단계 작업을 완료할 수 있는 대화형 인터페이스입니다.
- **공동 작업자 캠페인**: 캠페인 브리핑, 대상자 작성, 콘텐츠 생성, 여정 디자인 및 증명을 하나의 대화 경험으로 통합하는 AI 기반 애플리케이션입니다.

적격 고객이 점차 AI 비서 및 Experience Platform 에이전트에서 동료채팅으로 전환되고 있습니다. 평가판 자격, AI 크레딧 사용 방법 및 액세스 방법에 대해 알아보려면 [CX Enterprise Coworker 평가판](./agents/trial.md)을 읽어 보십시오.

동료 채팅을 실제로 보려면 [플레이그라운드에서 동료 채팅](./coworker/playground-coworker-chat.md)을 살펴보거나 [CJA 마이그레이션 데이터에 대한 AA 유효성 검사](./coworker/data-validation-aa-cja.md) 및 [전환 분석](./coworker/analytics-chat.md)과 같은 실제 사용 사례를 읽어 보십시오.

## MCP

[Adobe CX Coworker Gateway](./mcp/overview.md)은(는) CX Enterprise용 MCP(Unified Model Context Protocol) 종단점입니다. [!DNL Claude], [!DNL ChatGPT] 및 [!DNL Cursor]과(와) 같은 MCP 호환 클라이언트에게 Real-Time CDP, Experience Platform, Journey Optimizer, Customer Journey Analytics 및 Adobe Analytics을 포함하여 귀사에서 사용할 권한이 있는 제품 도구에 대한 단일 관리 연결을 제공합니다.

## 시작하기

### 액세스 요구 사항

AI Assistant 및 Experience Platform 에이전트를 사용하려면 Adobe 관리자가 적절한 권한을 부여해야 합니다. 요구 사항은 애플리케이션에 따라 다릅니다. 자세한 내용은 Agent Orchestrator 안내서의 [액세스](./agents/agent-orchestrator.md#access)를 참조하십시오.

### 개인정보보호 및 보안

AI Assistant 및 Experience Platform 에이전트는 샌드박스별 데이터 격리와 기존 액세스 제어 정책 준수 등 개인정보 보호, 보안 및 거버넌스를 전면에 내세우고 있습니다. 자세한 내용은 [AI Assistant의 개인 정보, 보안 및 거버넌스](./ai-assistant/privacy.md)를 참조하십시오.

## 모범 사례

AI Assistant 또는 동료 경험을 통해 최대의 가치를 얻으려면 다음 모범 사례를 따르십시오.

- 대상 및 관련 인사이트를 얻으려면 프롬프트에 **구체적으로**&#x200B;하십시오.
- 제공된 원본 인용과 추론 설명을 검토하여 **응답을 확인**&#x200B;합니다.
- **컨텍스트 설정을 사용**&#x200B;하여 가장 관련성이 높은 데이터 원본이 질문에 사용되었는지 확인하세요.
- **피드백을 제공**&#x200B;하여 시간이 지남에 따라 성능과 정확도를 개선하십시오.
- 보다 포괄적인 분석을 위해 여러 에이전트의 **통찰력을 결합**.

## 법적 고려 사항

AI Assistant는 현재 영어 응답만 지원하며 언어 모델이 가끔 실수를 할 수 있습니다. 제공된 정보를 항상 확인하고 각 응답에 포함된 추론 단계를 사용하여 생성 방법을 이해합니다. 자세한 내용은 [법적 고지 사항](./ai-assistant/legal-disclaimer.md)을 참조하세요.
