---
title: 创作AI内容透明度
description: 了解Adobe如何跨Adobe CX Enterprise应用程序将C2PA元数据自动附加到GenAI生成和GenAI编辑的内容。
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
  - id: ec4263d9-bf7c-44c7-b3f1-3e664861c8f2
source-git-commit: 4a9ab38cc3aa650dbb90639558d25f6acf707da5
workflow-type: tm+mt
source-wordcount: 1714
ht-degree: 1%

---


# 创作AI内容透明度

在整个2026年8月，Adobe正在逐步跨Adobe Creative Cloud、Adobe Document Cloud、Adobe Firefly和Adobe CX Enterprise应用程序推出C2PA元数据支持。

>[!NOTE]
>
>推出后，未来涉及使用AI创建或编辑内容的工作流将自动支持C2PA元数据。

本页详细介绍Adobe如何跨Adobe CX Enterprise应用程序处理C2PA元数据的自动连接。

新法规要求创新型人工智能技术提供商支持与GenAI生成和GenAI编辑的内容工作流相关的持久的、机器可读的披露，以提高透明度。

作为工具提供商，Adobe使用Adobe技术（包括Adobe工作流中受支持的第三方创作AI模型），将机器可读的C2PA元数据自动附加到GenAI生成的和GenAI编辑的内容。 [了解有关C2PA的更多信息](https://c2pa.org/)。

## 更改内容

Adobe将于2026年8月推出，将跨Adobe Creative Cloud、Adobe Document Cloud、Adobe Firefly和Adobe CX Enterprise应用程序引入C2PA元数据支持。

此版本包括：

* 自动将C2PA元数据附加到受支持的GenAI生成和GenAI编辑的内容。
* 支持内容类型，包括图像、视频、音频和文本。
* 在整个支持的Adobe工作流中保留C2PA元数据。

无需执行其他操作即可将C2PA元数据附加到符合条件的创作AI内容。

>[!NOTE]
>
>C2PA元数据不会影响内容的外观。 C2PA元数据和可见水印有不同的用途。 C2PA元数据提供机器可读的来源信息，而可见水印提供可视泄漏。 您可以根据业务需求和每个适用管辖区的法律要求，选择向内容添加可见水印。

## 哪些详细信息添加为C2PA元数据的一部分

自动附加的C2PA元数据可能包括以下信息：

* 使用的AI系统的名称和版本信息（例如，Adobe GenStudio、Adobe Firefly）
* 使用的AI模型（例如，Adobe Firefly）
* 用法：是否使用GenAI生成或编辑它
* 使用创作AI工具创建和/或修改内容的时间和日期
* 唯一标识符（可用于区分创作AI的每个用法）

## 跨内容supply chain的C2PA元数据

C2PA元数据设计为在Adobe应用程序和兼容的第三方平台之间移动时保持与受支持的内容相关联。

当内容被发布、分发或共享时，支持C2PA元数据或相关源技术的平台可以读取附加的元数据并向用户显示透明度信息。

在内容离开Adobe应用程序后，Adobe无法控制外部服务如何解释、显示或使用C2PA元数据。 客户应查阅各个发布平台的文档，以了解如何处理C2PA元数据。

## 可见水印

在某些情况下，在特定地理区域，组织可能会选择或要求显式标识GenAI生成或GenAI编辑的内容。

Adobe提供了有关使用通过Adobe应用程序支持的现有水印功能的[指南](https://helpx.adobe.com/cn/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)。 是否需要可见水印取决于组织的业务要求以及发布内容所在司法辖区的适用法律和法规。

>[!NOTE]
>
>C2PA元数据和可见水印有不同的用途。 C2PA元数据提供机器可读的来源信息，而可见水印提供组织可以选择应用的视觉公开。

## 可用性和版本

这些功能将在整个&#x200B;**2026年8月**&#x200B;日（在支持的Adobe CX Enterprise工作流中）推出。

>[!NOTE]
>
>推出后，未来涉及使用AI创建或编辑内容的工作流将自动支持C2PA元数据。

此版本包括：

### 自动C2PA元数据

C2PA元数据自动附加到受支持的GenAI生成和GenAI编辑的内容。 此功能默认处于启用状态，无法禁用。

### 水印指南

Adobe提供了[文档](https://helpx.adobe.com/cn/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)介绍如何使用受支持的Adobe应用程序中提供的现有水印功能，以供选择或需要应用可见标签的组织使用。

## 跨Adobe CX Enterprise支持的应用程序 {#supported-applications}

以下Adobe应用程序和服务提供了有关C2PA元数据如何以及何时附加到某些CX Enterprise应用程序中符合条件的内容的更多信息。

但是，在适用的情况下，所有Adobe CX Enterprise应用程序都会在受支持的资源通过Adobe工作流移动时继续保留现有C2PA元数据。 这有助于维护整个内容supply chain中的来源信息的完整性。

>[!NOTE]
>
>下面列出的每个应用程序的发行说明或指南都将在Experience League上的相应应用程序产品页面部分中提供。 当链接可用时，将用这些链接更新表格。 请参阅Experience League上的最新产品部分。

| 应用程序/解决方案 | 发行说明/指南 |
|---|---|
| Adobe Advertising Cloud | [文档](https://experienceleague.adobe.com/zh-hans/docs/advertising/creative/creative-studio/creative-studio-content-credentials) |
| Adobe Experience Manager (AEM) | [文档](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/c2pa-metadata-dynamic-media-openapi) |
| 用于内容生成的人工智能助手（Adobe Journey Optimizer/Adobe Campaign中的功能） | [文档](https://experienceleague.adobe.com/zh-hans/docs/journey-optimizer/using/content-management/generate-content/generative-c2pa-metadata) |
| Adobe Journey Optimizer B2B Ultimate | [文档](https://experienceleague.adobe.com/zh-hans/docs/journey-optimizer-b2b/user/content-management/assets/c2pa-metadata) |
| Adobe Journey Optimizer B2B Prime （又称Adobe Marketo Optimizer） | [文档](https://experienceleague.adobe.com/en/docs/marketo-optimizer/user/content/assets/c2pa-metadata) |
| Adobe Journey Optimizer B2C | |
| Adobe Campaign | |
| Adobe Commerce | [文档](https://experienceleague.adobe.com/zh-hans/docs/commerce/optimizer/manage-results/success-metrics#c2pa-metadata-on-exported-reports) |
| GenStudio for Performance Marketing | [文档](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/content/content-credentials) |
| Adobe Marketo Engage | [文档](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/demand-generation/images-and-files/c2pa-metadata) |
| Adobe Workfront | [文档](https://experienceleague.adobe.com/en/docs/workfront/using/documents/c2pa-metadata-overview) |
| CX Enterprise Co-worker Campaigns （以前称为HALO ） | [文档](https://experienceleague.adobe.com/zh-hans/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/c2pa-metadata) |

## 相关链接

* [可见水印指南](https://helpx.adobe.com/cn/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)
* [Adobe Inspect](https://contentauthenticity.adobe.com/inspect)
* [Adobe GenAI标签合规计划概述](https://helpx.adobe.com/cn/creative-cloud/apps/generative-ai/ai-content-labeling-faq.html)

## 常见问题

**哪些Adobe应用程序将C2PA元数据应用于已编辑或创建的创作AI内容？**

受支持的Adobe CX Enterprise应用程序自动将C2PA元数据附加到符合GenAI生成和GenAI编辑的内容中。 有关Adobe CX Enterprise应用程序的更多详细信息，请参阅[支持的应用程序](#supported-applications)部分。

**Adobe将C2PA元数据添加到哪些内容类型？**

从广义上讲，图像、音频、视频、文档和文本都在范围之内。 但是，请参阅[支持的应用程序](#supported-applications)部分中的文档，了解每个应用程序如何支持不同产品和内容类型的C2PA元数据。

**在编辑和发布过程中，Adobe CX中的哪些应用程序保留C2PA元数据？**

所有Adobe CX Enterprise应用程序都设计为可在内容通过兼容的Adobe工作流时保留C2PA元数据。 Adobe应用程序外部的保留取决于外部平台是否支持C2PA元数据。

**将多个GenAI生成的图像合并到单个图像时会发生什么情况？**

生成的C2PA元数据取决于使用的应用程序和工作流。 如果支持，Adobe将在整个编辑过程中保留来源信息。 有关每个应用程序中特定于工作流的行为的文档，请参阅[支持的应用程序](#supported-applications-across-adobe-cx-enterprise)部分。

**当来自Adobe和非Adobe应用程序的GenAI生成的图像被合并时，会发生什么情况？**

Adobe会保留工作流中可用且受支持的C2PA元数据。 只要适用，只要在Adobe工作流中使用GenAI编辑或创建适用的内容（图像、音频、视频、文本），Adobe就会使用最新信息更新基础元数据。 将多个源合并到一个新资产时，不会替换或丢失其基础元数据。 相反，新资产会获得自己的C2PA元数据，并且来自每个源的详细信息会保留在其中。 如果源已经拥有自己的C2PA元数据（无论它来自Adobe还是非Adobe工具），则历史记录会附加到该源。 这意味着，最终资产具有完整的概念：它自己的使用GenAI创建或编辑的记录，以及进入其中的每件作品的单独历史记录。

**Adobe CX应用程序中GenAI编辑和GenAI创建的工作流是否自动附加C2PA元数据？**

是的。 对于受支持的创作AI工作流，Adobe会自动附加C2PA元数据，这些元数据可识别内容是GenAI生成的还是GenAI编辑的，以及其他来源信息，例如时间戳、AI系统信息和唯一标识符。

**在整个内容supply chain中如何维护C2PA元数据？**

C2PA元数据是持久的元数据，旨在当它在兼容的Adobe应用程序和支持第三方平台之间移动时保持与支持的内容相关联。 外部服务确定在发布后如何显示附加的来源信息。

**组织如何在不破坏来源链的情况下添加自己的已验证信息？**

某些Adobe应用程序允许创建者和组织向现有C2PA元数据添加其他经过身份验证的信息，同时保留原始数据。 可用性因应用程序而异。

**是否可以关闭C2PA元数据的自动附加？**

没有。 新的创新型人工智能透明度法律要求提供创新型人工智能工具（包括Adobe）的公司将持久元数据附加到使用创新型人工智能生成或编辑的符合条件的内容。 无法关闭C2PA元数据的自动附加。

**在8月版本发布之前，使用创作AI创建/编辑的内容发生了什么情况？**

在2026年8月版本之前使用创作AI工具创建或编辑的内容没有附加自动C2PA元数据。 但是，在Firefly Web和之前应用了C2PA元数据的其他应用程序中创建的内容将继续附加这些内容。

**客户如何检查内容是否附加了C2PA元数据？**

客户可以通过将内容上传到[Adobe Inspect](https://contentauthenticity.adobe.com/inspect)页面来检查该内容是否附加了C2PA元数据。

**发布或共享内容后，外部平台如何显示C2PA元数据？**

随着内容在发布平台、社交媒体渠道、电子邮件服务和其他数字生态系统中移动，支持C2PA元数据或相关来源技术的下游服务可能能够读取附加的元数据并根据该信息选择显示披露或指标。 Adobe无法控制外部平台如何显示、解释或应用与附加的C2PA元数据关联的披露。 有关特定平台如何处理来源信息的最新信息，客户应直接查看该平台的准则。

**这些更改是否会增加Adobe产品或订阅的成本？**

没有。 C2PA元数据不会影响Adobe产品的成本。
