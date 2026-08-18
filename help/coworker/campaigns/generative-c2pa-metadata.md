---
description: Coworker Campaigns에서 AI가 생성하고 편집한 이미지에 대해 별도의 작업 없이 C2PA 메타데이터(Content Credentials)를 자동으로 첨부하고 보존하는 방법에 대해 알아봅니다.
title: 동료 캠페인의 C2PA 메타데이터
hide: true
source-git-commit: 785b5d106cb029d68506c90385786cbdae164991
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 2%

---

# 동료 캠페인의 C2PA 메타데이터 {#overview}

생성 AI 투명성을 중심으로 새로운 법이 등장하고 있으며, Adobe은 관할권 전반에서 적용 가능한 요구 사항을 충족하기 위해 노력하고 있습니다. [C2PA 메타데이터](https://c2pa.org/)&#x200B;(Content Credentials이라고도 함)은 Adobe이 이러한 법률의 요구 사항을 충족하기 위해 사용하는 증명 도구입니다.

C2PA 메타데이터는 콘텐츠의 한 부분이 생성되거나 편집되는 방식을 기록하는 보이지 않는 지속적인 메타데이터입니다. 동료 캠페인에서 생성 AI 도구를 사용하여 이미지를 생성하거나 편집하면 C2PA 메타데이터가 해당 이미지에 자동으로 첨부됩니다. 사용자 측에서는 아무 작업도 필요하지 않습니다.

## C2PA 메타데이터를 첨부하는 작업 {#cc-workflows}

다음 표에서는 Coworker Campaign에서 이미지 생성에 수행된 이미지 작업을 기반으로 C2PA 메타데이터가 첨부되는 시기를 요약합니다.

| 작업 | 설명 | C2PA 메타데이터가 첨부되었습니까? | 사용 사례 예 |
| --- | --- | --- | --- |
| **이미지 생성** | 텍스트 프롬프트 또는 참조 이미지에서 새 이미지를 생성하거나 기존 이미지에서 유사한 이미지를 생성합니다. | 항상 이미지는 생성 AI에 의해 생성되므로 항상 새로운 C2PA 메타데이터를 전달합니다. | 이메일 캠페인에 대한 배너 이미지는 원하는 시각적 개체를 설명하는 텍스트 프롬프트에서 생성됩니다. |
| **이미지 자르기**(가운데 또는 스마트 자르기) | 이미지를 요청된 치수로 조정 | 소스 이미지에 이미 C2PA 메타데이터가 있는 경우에만 해당합니다. 자르기는 이미지의 픽셀을 다시 만드므로 일반적으로 해당 C2PA 메타데이터는 지워지므로 Coworker Campaigns의 이미지 생성은 자르기 전에 소스 이미지에서 읽은 다음 자른 결과에 다시 빌드하고 다시 연결합니다. 자르기 자체로는 새로운 생성 AI 작업이 추가되지 않으며 기존 AI 작업을 유지합니다. | 생성된 배너 이미지는 웹 페이지에 맞게 잘립니다. C2PA 메타데이터는 자르기를 통해 유지됩니다. <br> 푸시 알림 배경으로 사용되는 업로드된 스톡 사진은 화면에 맞게 잘립니다. 스톡 사진은 생성 AI 작업을 수행하지 않으므로 C2PA 메타데이터가 생성되지 않습니다. |
| **텍스트 오버레이 추가** | 배경 이미지 위에 생성된 텍스트 렌더링 | 배경 이미지에 이미 C2PA 메타데이터가 있는 경우에만 해당합니다. 오버레이를 렌더링하면 배경과 텍스트에서 새 이미지가 생성되며, 이렇게 하면 일반적으로 해당 C2PA 메타데이터가 지워지므로 Coworker Campaigns의 이미지 생성은 배경 이미지에서 미리 읽은 다음 다시 빌드하고 결과에 다시 첨부합니다. 오버레이 단계는 새로운 생성 AI 작업을 추가하지 않습니다. | 홍보 헤드라인은 랜딩 페이지에 대해 생성된 배경 이미지에 텍스트 오버레이로 렌더링됩니다. 배경 이미지의 C2PA 메타데이터는 유지됩니다. |
| **오버레이 이미지** | 두 개 이상의 이미지를 함께 합성 | 소스 이미지에 C2PA 메타데이터가 있으면 결합된 이미지가 모든 이미지를 전달하여 단일 C2PA 메타데이터 세트로 병합됩니다. 합성은 일반적으로 해당 C2PA 메타데이터를 지우는 소스에서 새 이미지를 생성하므로 동료 캠페인의 이미지 생성은 합성하기 전에 각각을 읽은 다음 생성 AI 작업에 기여한 모든 소스를 나열하는 하나의 결합된 C2PA 메타데이터 레코드를 빌드합니다. | 생성된 제품 이미지는 이메일 헤더에 대해 생성된 배경과 합성됩니다. 이 결과는 생성된 AI 소스를 모두 반영하는 C2PA 메타데이터를 전달합니다. <br> 업로드된 두 개의 브랜드 사진은 하나의 콜라주에 합성됩니다. 두 소스 모두 생성 AI 작업을 수행하지 않으므로 C2PA 메타데이터가 생성되지 않습니다. |

## 컨텐츠 유형 및 해당 범위 {#cc-content-types}

* **이미지**: 적용됨. C2PA 메타데이터는 생성 AI로 이미지가 생성될 때 첨부되며, 동료 캠페인에서 이미지 생성으로 수행된 자르기, 텍스트 오버레이 및 이미지 오버레이 작업을 통해 보존됩니다.
* **텍스트**: 적용할 수 없습니다. 복사 생성, 번역 및 브랜드 정렬 제안과 같은 Coworker Campaign에서 이미지 생성의 텍스트 전용 출력에는 C2PA 메타데이터가 필요하지 않습니다.

## 콘텐츠가 이동할 때 수행되는 작업 {#cc-content-moves}

동료 캠페인은 지원되는 이미지 자산과 연결된 Content Credentials을 유지합니다. 이미지가 Content Credentials 를 포함하고 동료가 Campaign으로 가져오는 경우 해당 자산이 생성된 캠페인 콘텐츠 및 아웃바운드 이메일 경험에 사용될 때 해당 자격 증명이 유지됩니다. [C2PA 메타데이터에 대해 자세히 알아보세요](https://helpx.adobe.com/kr/firefly/using/content-credentials.html){target="_blank"}.

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

>[!MORELIKETHIS]
>
>[Adobe Experience Cloud 생성 AI 사용자 지침](https://www.adobe.com/kr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}
