---
description: 了解同事营销活动如何自动附加并保留图像上的C2PA元数据(Content Credentials)，从生成一直到电子邮件投放。
title: 同事营销活动中的C2PA元数据
hide: true
source-git-commit: 9796ac7d3d55e7a278414d44a214bfdf5311d727
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 6%

---

# 同事营销活动中的C2PA元数据 {#overview}

围绕创新型人工智能透明度的新法律正在出现，Adobe正在努力满足跨司法辖区的适用要求。 [C2PA元数据](https://c2pa.org/)（也称为Content Credentials）是Adobe用于满足这些法律要求的源工具。

C2PA元数据是持久的、不可见的元数据，记录一段内容的创建或编辑方式。 在Co-worker Campaigns中使用创作AI工具生成或编辑图像时，C2PA元数据会自动附加到该图像。 您无需执行任何操作。

>[!BEGINSHADEBOX]

## 电子邮件营销活动中的Content Credentials {#content-credentials-email}

在电子邮件促销活动中发送的图像将其Content Credentials保持不变，因此收件人可以直接从投放的电子邮件中验证任何图像的来源和真实性。

>[!ENDSHADEBOX]

## 附加C2PA元数据的操作 {#cc-workflows}

下表基于在同事营销活动中生成图像时执行的图像操作，总结了附加C2PA元数据的时间。

| 操作 | 描述 | 是否附加C2PA元数据？ | 用例示例 |
| --- | --- | --- | --- |
| **生成图像** | 从文本提示或参考图像创建新图像，或从现有图像生成类似图像。 | 一直。 由于图像是由创成式人工智能生成的，因此它总是带有新的C2PA元数据。 | 从描述所需视觉效果的文本提示生成电子邮件促销活动的横幅图像。 |

## 内容类型及其范围 {#cc-content-types}

* **图像**：已覆盖。 使用创作AI生成图像时，会附加C2PA元数据，并通过在Co-worker Campaigns中通过图像生成执行的裁切、文本叠加和图像叠加操作来保留。
* **文本**：不适用。 在合作营销活动中生成图像的纯文本输出（如副本生成、翻译和品牌对齐建议）不需要C2PA元数据。

## 内容移动时发生的情况 {#cc-content-moves}

同事营销活动会保留与支持的图像资源关联的Content Credentials。 如果导入到同事营销活动中的图像包含Content Credentials，则在生成的营销活动内容和出站电子邮件体验中使用资产时，将保留这些凭据。

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

## 其他资源

* [了解有关C2PA元数据的更多信息](https://helpx.adobe.com/cn/firefly/using/content-credentials.html){target="_blank"}

* [Adobe Experience Cloud创作AI用户准则](https://www.adobe.com/cn/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}

* [护栏和限制](https://experienceleague.adobe.com/zh-hans/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails){target="_blank"}
