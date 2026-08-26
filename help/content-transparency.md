---
title: 생성 AI 콘텐츠 투명도
description: Adobe에서 Adobe CX 엔터프라이즈 애플리케이션 전반에 걸쳐 GenAI가 생성한 콘텐츠 및 GenAI가 편집한 콘텐츠에 C2PA 메타데이터를 자동으로 연결하는 방법에 대해 알아봅니다.
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
  - id: ec4263d9-bf7c-44c7-b3f1-3e664861c8f2
source-git-commit: 1fe34a4a2056a15c7417f8794eba5981481b0111
workflow-type: tm+mt
source-wordcount: 1714
ht-degree: 1%

---


# 생성 AI 콘텐츠 투명도

2026년 8월 현재 Adobe은 Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly 및 Adobe CX 엔터프라이즈 애플리케이션에서 C2PA 메타데이터 지원을 점차 제공하고 있습니다.

>[!NOTE]
>
>롤아웃 이후 AI를 사용하여 컨텐츠를 만들거나 편집하는 것과 관련된 향후 워크플로우는 자동으로 C2PA 메타데이터를 지원합니다.

이 페이지에서는 Adobe이 Adobe CX 엔터프라이즈 애플리케이션 전반에 걸쳐 C2PA 메타데이터의 자동 첨부 파일을 처리하는 방법에 대한 세부 정보를 다룹니다.

새로운 규정에서는 생성 AI 기술 제공업체가 GenAI 생성 및 GenAI 편집 콘텐츠 워크플로우와 관련된 지속적이고 기계 판독이 가능한 공개를 지원하여 투명성을 높여야 합니다.

도구 제공업체로서 Adobe은 Adobe 기술(Adobe 워크플로 내에서 지원되는 타사 생성 AI 모델 포함)을 사용하여 GenAI가 생성하고 GenAI가 편집한 컨텐츠에 기계 판독이 가능한 C2PA 메타데이터를 자동으로 첨부합니다. [C2PA에 대해 자세히 알아보기](https://c2pa.org/).

## 변경 사항

2026년 8월에 출시되는 Adobe은 Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly 및 Adobe CX 엔터프라이즈 애플리케이션 전반에 걸쳐 C2PA 메타데이터 지원을 도입할 예정입니다.

이번 릴리스에는 다음이 포함됩니다.

* 지원되는 GenAI 생성 및 GenAI 편집 콘텐츠에 C2PA 메타데이터를 자동으로 첨부합니다.
* 이미지, 비디오, 오디오 및 텍스트를 포함한 콘텐츠 유형을 지원합니다.
* 지원되는 Adobe 워크플로 전체에서 C2PA 메타데이터 보존.

자격 있는 생성 AI 콘텐츠에 C2PA 메타데이터를 첨부하기 위해 추가 작업은 필요하지 않습니다.

>[!NOTE]
>
>C2PA 메타데이터는 콘텐츠의 모양에 영향을 주지 않습니다. C2PA 메타데이터와 표시되는 워터마크는 서로 다른 용도로 사용됩니다. C2PA 메타데이터는 기계가 읽을 수 있는 증명 정보를 제공하는 반면, 보이는 워터마크는 시각적 공개를 제공합니다. 비즈니스 요구 사항 및 각 해당 관할권의 법적 요구 사항에 따라 콘텐츠에 시각적 워터마크를 추가할 수 있습니다.

## C2PA 메타데이터의 일부로 추가된 세부 정보

자동으로 첨부된 C2PA 메타데이터는 다음과 같은 정보를 포함할 수 있습니다.

* 사용된 AI 시스템의 이름 및 버전 정보(예: Adobe GenStudio, Adobe Firefly)
* 사용된 AI 모델(예: Adobe Firefly)
* 사용법: GenAI를 사용하여 생성되었는지 또는 편집했는지 여부
* 콘텐츠 생성 및/또는 생성 AI 도구를 사용한 수정 시간과 날짜
* 고유 식별자(생성 AI의 각 사용을 구분하는 데 사용할 수 있음)

## 컨텐츠 supply chain의 C2PA 메타데이터

C2PA 메타데이터는 Adobe 애플리케이션과 호환되는 타사 플랫폼 간에 이동할 때 지원되는 콘텐츠와 연결된 상태를 유지하도록 설계되었습니다.

콘텐츠가 게시되거나 배포되거나 공유됨에 따라 C2PA 메타데이터 또는 관련 증명 기술을 지원하는 플랫폼은 첨부된 메타데이터를 읽고 사용자에게 투명도 정보를 표시할 수 있습니다.

Adobe은 컨텐츠가 Adobe 애플리케이션을 떠난 후 외부 서비스가 C2PA 메타데이터를 해석, 표시 또는 사용하는 방법을 제어하지 않습니다. 고객은 개별 게시 플랫폼에 대한 설명서를 참조하여 C2PA 메타데이터가 처리되는 방법을 이해해야 합니다.

## 워터마크 표시

일부 상황과 특정 지역에서 조직은 GenAI가 생성한 콘텐츠 또는 GenAI가 편집한 콘텐츠를 시각적으로 식별하도록 선택하거나 요구될 수 있습니다.

Adobe은 Adobe 애플리케이션을 통해 지원되는 기존 워터마크 기능 사용에 대한 [지침](https://helpx.adobe.com/kr/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)을 제공합니다. 가시적인 워터마크가 필요한지 여부는 조직의 비즈니스 요구 사항과 콘텐츠가 게시되는 관할권의 해당 법률 및 규정에 따라 다릅니다.

>[!NOTE]
>
>C2PA 메타데이터와 표시되는 워터마크는 서로 다른 용도로 사용됩니다. C2PA 메타데이터는 기계가 읽을 수 있는 증명 정보를 제공하는 반면, 보이는 워터마크는 조직이 적용하도록 선택할 수 있는 시각적 개시를 제공합니다.

## 가용성 및 릴리스

이러한 기능은 지원되는 Adobe CX Enterprise 워크플로우에서 **2026년 8월** 동안 롤아웃됩니다.

>[!NOTE]
>
>롤아웃 이후 AI를 사용하여 컨텐츠를 만들거나 편집하는 것과 관련된 향후 워크플로우는 자동으로 C2PA 메타데이터를 지원합니다.

이 릴리스에는 다음이 포함됩니다.

### 자동 C2PA 메타데이터

지원되는 GenAI 생성 및 GenAI 편집 콘텐츠에 C2PA 메타데이터가 자동으로 첨부됩니다. 이 기능은 기본적으로 활성화되어 있으며 비활성화할 수 없습니다.

### 워터마크 지침

Adobe은 시각적 레이블을 선택하거나 적용할 필요가 있는 조직을 위해 지원되는 Adobe 애플리케이션에서 사용할 수 있는 기존 워터마크 기능을 사용하는 방법을 설명하는 [설명서](https://helpx.adobe.com/kr/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)를 제공합니다.

## Adobe CX Enterprise에서 지원되는 애플리케이션 {#supported-applications}

다음 Adobe 애플리케이션 및 서비스는 특정 CX 엔터프라이즈 앱 내의 검증된 컨텐츠에 C2PA 메타데이터를 연결하는 방법과 시기에 대한 추가 정보를 제공합니다.

그러나 지원되는 자산이 Adobe 워크플로를 통해 이동함에 따라 해당되는 경우 모든 Adobe CX 엔터프라이즈 애플리케이션은 기존 C2PA 메타데이터를 계속 보존합니다. 이렇게 하면 컨텐츠 supply chain 전체에서 증명 정보의 무결성을 유지하는 데 도움이 됩니다.

>[!NOTE]
>
>아래에 나열된 각 애플리케이션에 대한 릴리스 노트 또는 지침은 해당 애플리케이션 제품 페이지 섹션의 Experience League에서 제공됩니다. 표가 업데이트되고 링크가 제공됩니다. Experience League에 대한 최신 제품 섹션을 참조하십시오.

| 애플리케이션/솔루션 | 릴리스 노트/지침 |
|---|---|
| Adobe Advertising Cloud | [설명서]&#x200B;(https://experienceleague.adobe.com/ko/docs/advertising/creative/creative-studio/creative-studio-content-credentials) |
| AEM(Adobe Experience Manager) | [설명서]&#x200B;(https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/c2pa-metadata-dynamic-media-openapi) |
| 콘텐츠 생성을 위한 AI 지원(Adobe Journey Optimizer/Adobe Campaign의 기능) | [설명서]&#x200B;(https://experienceleague.adobe.com/ko/docs/journey-optimizer/using/content-management/generate-content/generative-c2pa-metadata) |
| Adobe Journey Optimizer Ultimate | [설명서]&#x200B;(https://experienceleague.adobe.com/ko/docs/journey-optimizer-b2b/user/content-management/assets/c2pa-metadata) |
| Adobe Journey Optimizer B2B Prime(Adobe Marketo Optimizer) | [설명서]&#x200B;(https://experienceleague.adobe.com/en/docs/marketo-optimizer/user/content/assets/c2pa-metadata) |
| Adobe Journey Optimizer | |
| Adobe Campaign | |
| Adobe Commerce | [설명서]&#x200B;(https://experienceleague.adobe.com/ko/docs/commerce/optimizer/manage-results/success-metrics#c2pa-metadata-on-exported-reports) |
| GenStudio for Performance Marketing | [설명서]&#x200B;(https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/content/content-credentials) |
| Adobe Marketo Engage | [설명서]&#x200B;(https://experienceleague.adobe.com/ko/docs/marketo/using/product-docs/demand-generation/images-and-files/c2pa-metadata) |
| Adobe Workfront | [설명서](https://experienceleague.adobe.com/en/docs/workfront/using/documents/c2pa-metadata-overview) |
| CX Enterprise Coworker 캠페인(이전 명칭 HALO) | [설명서](https://experienceleague.adobe.com/ko/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/c2pa-metadata) |

## 관련 링크

* [워터마크 가이드 표시](https://helpx.adobe.com/kr/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)
* [Adobe Inspect](https://contentauthenticity.adobe.com/inspect)
* [Adobe GenAI Labeling Compliance Initiative 개요](https://helpx.adobe.com/kr/creative-cloud/apps/generative-ai/ai-content-labeling-faq.html)

## 자주 묻는 질문

**어떤 Adobe 앱에서 C2PA 메타데이터를 생성 AI가 편집하거나 만든 콘텐츠에 적용합니까?**

지원되는 Adobe CX 엔터프라이즈 애플리케이션은 적합한 GenAI 생성 및 GenAI 편집 콘텐츠에 C2PA 메타데이터를 자동으로 첨부합니다. Adobe CX 엔터프라이즈 응용 프로그램에 대한 자세한 내용은 [지원되는 응용 프로그램](#supported-applications) 섹션을 참조하십시오.

**Adobe에서 C2PA 메타데이터를 추가하는 콘텐츠 유형은 무엇입니까?**

넓게는 이미지, 오디오, 비디오, 문서 및 텍스트가 범위에 있습니다. 그러나 [지원되는 응용 프로그램](#supported-applications) 섹션의 설명서를 참조하여 각 응용 프로그램이 다양한 제품 및 콘텐츠 유형에서 C2PA 메타데이터를 지원하는 방법을 확인하십시오.

**편집 및 게시 전체에서 C2PA 메타데이터를 보존하는 Adobe CX의 응용 프로그램은 무엇입니까?**

모든 Adobe CX 엔터프라이즈 애플리케이션은 호환하는 Adobe 워크플로우를 통해 콘텐츠가 이동할 때 C2PA 메타데이터를 보존하도록 설계되었습니다. Adobe 애플리케이션 외부의 보존은 외부 플랫폼이 C2PA 메타데이터를 지원하는지 여부에 따라 달라집니다.

**GenAI에서 생성한 여러 이미지를 하나의 이미지로 결합하면 어떻게 됩니까?**

결과 C2PA 메타데이터는 사용되는 애플리케이션 및 워크플로에 따라 다릅니다. 지원되는 경우 Adobe은 편집 프로세스 전체에서 조달 정보를 유지합니다. 각 앱의 워크플로우별 동작에 대한 설명서는 [지원되는 응용 프로그램](#supported-applications-across-adobe-cx-enterprise) 섹션을 참조하십시오.

**Adobe 및 Adobe 이외의 애플리케이션에서 GenAI가 생성한 이미지가 결합되면 어떻게 됩니까?**

Adobe은 워크플로우 내에서 사용 가능하고 지원되는 C2PA 메타데이터를 유지합니다. 해당되는 경우 Adobe은 Adobe 워크플로 내에서 GenAI를 사용하여 해당 콘텐츠(이미지, 오디오, 비디오, 텍스트)를 편집하거나 만들 때마다 기본 메타데이터를 최신 정보로 업데이트합니다. 여러 소스를 하나의 새 에셋으로 결합하면 기본 메타데이터가 대체되거나 손실되지 않습니다. 대신 새 에셋은 자체 C2PA 메타데이터를 가져오고, 각 소스의 세부 정보를 해당 에셋 내부에 유지합니다. 소스에 이미 자체 C2PA 메타데이터가 있는 경우(Adobe에서 가져왔든 비 Adobe 도구에서 가져왔든) 해당 기록은 연결된 상태로 유지됩니다. 이는 최종 자산이 완전한 그림을 가지고 있다는 것을 의미합니다: GenAI로 생성 또는 편집된 자신의 기록과 거기에 들어간 각 조각의 개별 기록.

**Adobe CX 응용 프로그램에서 GenAI가 편집하고 GenAI가 만든 워크플로에 C2PA 메타데이터가 자동으로 첨부됩니까?**

예. 지원되는 생성 AI 워크플로의 경우 Adobe은 콘텐츠가 GenAI에서 생성되었는지 또는 GenAI에서 편집되었는지 여부를 식별하는 C2PA 메타데이터와 타임스탬프, AI 시스템 정보 및 고유 식별자와 같은 다른 증명 정보를 자동으로 첨부합니다.

**컨텐츠 supply chain 전체에서 C2PA 메타데이터는 어떻게 유지 관리됩니까?**

C2PA 메타데이터는 호환되는 Adobe 애플리케이션과 지원되는 타사 플랫폼 간에 이동할 때 지원되는 콘텐츠와 연결된 상태를 유지하도록 설계된 지속적인 메타데이터입니다. 외부 서비스는 게시 후 첨부된 조달 정보가 표시되는 방식을 결정합니다.

**조직이 provenance chain을 중단하지 않고 인증된 정보를 추가하려면 어떻게 해야 합니까?**

일부 Adobe 애플리케이션을 사용하면 생성자 및 조직이 provenance를 유지하면서 기존 C2PA 메타데이터에 인증된 정보를 추가할 수 있습니다. 사용 가능 여부는 애플리케이션에 따라 다릅니다.

**C2PA 메타데이터의 자동 첨부 기능을 해제할 수 있습니까?**

아니요. 새로운 생성 AI 투명성 법안은 Adobe을 비롯한 생성 AI 도구를 제공하는 기업이 생성 AI로 생성 또는 편집된 적격 콘텐츠에 내구성 있는 메타데이터를 첨부하도록 했다. C2PA 메타데이터의 자동 첨부 기능을 끌 수 없습니다.

**8월 릴리스 전에 생성 AI로 생성/편집한 콘텐츠는 어떻게 됩니까?**

2026년 8월 릴리스 이전에 생성 AI 도구로 생성 또는 편집된 콘텐츠에는 자동 C2PA 메타데이터가 첨부되지 않습니다. 그러나 Firefly 웹 및 이전에 C2PA 메타데이터가 적용된 기타 앱에서 생성된 콘텐츠에는 해당 콘텐츠가 계속 첨부되어 있습니다.

**고객이 콘텐츠에 C2PA 메타데이터가 첨부되어 있는지 어떻게 확인할 수 있습니까?**

고객은 [Adobe Inspect](https://contentauthenticity.adobe.com/inspect) 페이지에 업로드하여 콘텐츠에 C2PA 메타데이터가 첨부되어 있는지 여부를 확인할 수 있습니다.

**콘텐츠를 게시하거나 공유하면 외부 플랫폼에 C2PA 메타데이터가 어떻게 표시됩니까?**

콘텐츠가 게시 플랫폼, 소셜 미디어 채널, 이메일 서비스 및 기타 디지털 생태계 전반에서 이동할 때 C2PA 메타데이터 또는 관련 증명 기술을 지원하는 다운스트림 서비스는 첨부된 메타데이터를 읽고 해당 정보를 기반으로 공개 또는 지표를 표시하도록 선택할 수 있습니다. Adobe은 외부 플랫폼이 연결된 C2PA 메타데이터와 연결된 공개를 표시, 해석 또는 적용하는 방법을 제어하지 않습니다. 특정 플랫폼이 조달 정보를 처리하는 방법에 대한 최신 정보는 고객이 해당 플랫폼의 지침을 직접 확인해야 합니다.

**이러한 변경 사항으로 인해 Adobe 제품 또는 구독의 비용이 증가합니까?**

아니요. C2PA 메타데이터는 Adobe 제품 비용에 영향을 주지 않습니다.
