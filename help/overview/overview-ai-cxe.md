---
title: CX Enterprise의 AI 정보
description: CX Enterprise 애플리케이션에서 생성 및 agentic AI를 사용할 수 있는 위치를 알아보고 시작하기 전에 액세스, 개인 정보 및 보안 요구 사항을 검토하십시오.
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
    internal-label: CX Enterprise Coworker
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
    internal-label: AI Tools
role_v2:
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: fccf9111460413fe5b89229564a682827152b1ab
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 3%
---
# CX Enterprise의 AI 정보

Adobe CX 엔터프라이즈 애플리케이션은 두 가지 상호 보완적인 방식으로 AI를 사용합니다. 즉, 콘텐츠를 직접 만들거나 답변을 얻으라는 메시지를 표시하는 **생성 AI**&#x200B;와 사용자를 대신하여 여러 단계 작업을 계획하고 수행하는 **아젠틱 AI**&#x200B;입니다. 다음 항목에서는 CX Enterprise에서 각 유형의 AI를 사용할 수 있는 위치를 광범위하게 설명합니다.

## 이 섹션에서 다루는 내용

- **[생성 AI 정보](./generative-ai.md)** CX 엔터프라이즈 애플리케이션에서 현재 생성 AI 및 AI Assistant 기능을 제공하는 카탈로그로, 이를 통해 제품 포트폴리오에서 genAI의 범위를 한눈에 확인할 수 있습니다.
- **[에이전트 AI 정보](./agentic-ai.md)**&#x200B;에서는 Experience Platform 에이전트와 Agent Orchestrator의 작동 방식, 기존 CX 엔터프라이즈 응용 프로그램과 AI 우선 응용 프로그램의 에이전트 간의 차이점 및 각 에이전트에서 사용 가능한 에이전트를 설명합니다.
- **[Agentic AI 모니터링](./monitoring.md)**&#x200B;은(는) 조직 전반에서 에이전트 채택, 사용 및 피드백을 추적하는 데 사용하는 Center of Excellence 팀과 기타 거버넌스 이해 당사자를 다룹니다.
- **[AI 크레딧 사용량](./ai-credit-consumption.md)**&#x200B;에서는 에이전트 작업 및 동료 입력이 AI 크레딧을 사용하는 방법을 설명하며, 에이전트 및 작업 유형별 예상 비율을 설명합니다. 따라서 사용을 계획하고 예산을 편성할 수 있습니다.
- **[생성 AI 콘텐츠 투명도](../content-transparency.md)**&#x200B;는 Adobe이 GenAI가 생성한 콘텐츠 및 GenAI가 편집한 콘텐츠에 C2PA 메타데이터를 자동으로 첨부하는 방법을 설명하여 조직의 공개 의무를 이해할 수 있도록 지원합니다.
- **[CX 엔터프라이즈 에이전트 도구](https://experienceleague.adobe.com/ko/docs/cx-enterprise-agentic-tools/using/overview)**&#x200B;는 CX 엔터프라이즈 에이전트를 확장하는 추가 에이전트 기술 및 도구에 대한 비디오 튜토리얼입니다.

## 시작하기에 앞서 {#before-you-begin}

팀에서 Coworker, AI Assistant 또는 Agentic AI를 사용하기 전에 다음 액세스, 개인정보 및 보안 요구 사항을 검토하십시오.

### 액세스 요구 사항

사용자가 AI Assistant 및 Experience Platform 에이전트에 액세스하려면 Adobe 관리자가 적절한 권한을 부여해야 합니다. 요구 사항은 애플리케이션에 따라 다릅니다. 자세한 내용은 Agent Orchestrator 안내서의 [액세스](../agents/agent-orchestrator.md#access)를 참조하십시오. CX Enterprise Coworker 액세스는 자격 기반 평가판을 통해 별도로 롤아웃됩니다. 조직에서 액세스할 수 있는 방법을 알아보려면 [동료 평가판](../agents/trial.md)을 참조하세요.

### 개인정보보호 및 보안

AI Assistant 및 Experience Platform 에이전트는 샌드박스별 데이터 격리와 기존 액세스 제어 정책을 포함하여 개인 정보, 보안 및 거버넌스의 우선순위를 지정합니다. 자세한 내용은 [AI Assistant의 개인 정보, 보안 및 거버넌스](../ai-assistant/privacy.md)를 참조하십시오.

## 시작 위치

1. 사용 가능한 두 가지 형태의 AI와 각 AI가 이미 사용 허가된 애플리케이션에 있는 위치를 이해하려면 **생성 AI 정보** 및 **무산소 AI 정보**&#x200B;를 읽어 보십시오.
1. 사용이 비용으로 변환되는 방식을 이해하려면 **AI 크레딧 소비**&#x200B;를 읽어 보십시오. 이를 통해 금융 및 조달에서 기대치를 설정할 수 있습니다.
1. 거버넌스 팀에 대한 **Agentic AI 모니터링** 대시보드 권한을 설정하여 첫 날부터 채택 및 사용을 볼 수 있도록 합니다.
1. 팀이 게시하는 AI 생성 콘텐츠에 자동으로 적용되는 공개 내용을 이해하려면 **생성 AI 콘텐츠 투명도**&#x200B;를 읽어 보십시오.
1. Adobe 관리자와 협력하여 위의 **시작하기 전에** 액세스 요구 사항을 완료한 다음, AI Assistant, Agent Orchestrator 및 CX Enterprise Coworker에 대한 실습 지침을 위해 사용자에게 CX Enterprise 애플리케이션의 [AI](../home.md)를 안내합니다.
