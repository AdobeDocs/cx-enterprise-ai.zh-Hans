---
description: 了解同事营销活动如何在AI生成和编辑的图像上自动附加和保留C2PA元数据(Content Credentials)，而无需执行任何操作。
title: 同事营销活动中的C2PA元数据
hide: true
source-git-commit: 785b5d106cb029d68506c90385786cbdae164991
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 2%

---

# 同事营销活动中的C2PA元数据 {#overview}

围绕创新型人工智能透明度的新法律正在出现，Adobe正在努力满足跨司法辖区的适用要求。 [C2PA元数据](https://c2pa.org/)（也称为Content Credentials）是Adobe用于满足这些法律要求的源工具。

C2PA元数据是持久的、不可见的元数据，记录一段内容的创建或编辑方式。 在Co-worker Campaigns中使用创作AI工具生成或编辑图像时，C2PA元数据会自动附加到该图像。 您无需执行任何操作。

## 附加C2PA元数据的操作 {#cc-workflows}

下表基于在同事营销活动中生成图像时执行的图像操作，总结了附加C2PA元数据的时间。

| 操作 | 描述 | 是否附加C2PA元数据？ | 用例示例 |
| --- | --- | --- | --- |
| **生成图像** | 从文本提示或参考图像创建新图像，或从现有图像生成类似图像。 | 一直。 由于图像是由创成式人工智能生成的，因此它总是带有新的C2PA元数据。 | 从描述所需视觉效果的文本提示生成电子邮件促销活动的横幅图像。 |
| **裁切图像**（居中裁切或智能裁切） | 根据请求的尺寸调整图像 | 仅当源图像已具有C2PA元数据时。 裁剪会重新创建图像的像素，这通常会擦除该C2PA元数据，因此Co-worker Campaigns中的图像生成会在裁剪之前从源图像读取该元数据，然后重新构建它并重新附加到裁剪的结果。 裁剪本身不会添加新的创新型人工智能操作；而是保留现有操作。 | 生成的横幅图像会被裁剪以适合网页：通过裁剪保留C2PA元数据。<br> 用作推送通知背景的上传库存照片会被裁剪以适合屏幕：由于库存照片不执行创作AI操作，因此不会创建C2PA元数据。 |
| **添加文本叠加** | 在背景图像上渲染生成的文本 | 仅当背景图像已具有C2PA元数据时。 渲染叠加图时，将从背景加上文本生成新图像，文本通常会擦除该C2PA元数据，因此Co-worker Campaigns中的图像生成会预先从背景图像读取该元数据，然后重新构建该图像，并将其重新附加到结果。 叠加步骤不会添加新的创作AI操作。 | 促销标题被呈现为在登陆页生成的背景图像上的文本叠加：来自背景图像的C2PA元数据被保留。 |
| **覆盖图像** | 将两个或多个图像组合在一起 | 如果任何源图像具有C2PA元数据，则组合图像携带所有该元数据，并合并到单个C2PA元数据集中。 合成操作会从源中生成一个新图像，它通常会擦除该C2PA元数据，因此Co-worker Campaigns中的图像生成操作会在合成之前读取每个元数据，然后生成一个合并的C2PA元数据记录，其中列出每个有助于生成人工智能操作的源。 | 生成的产品图像与为电子邮件标题生成的背景合成：结果携带反映两个生成AI源的C2PA元数据。<br> 将两张上传的品牌照片合成一个拼贴：由于两个来源都不执行创作AI操作，因此不会创建C2PA元数据。 |

## 内容类型及其范围 {#cc-content-types}

* **图像**：已覆盖。 使用创作AI生成图像时，会附加C2PA元数据，并通过在Co-worker Campaigns中通过图像生成执行的裁切、文本叠加和图像叠加操作来保留。
* **文本**：不适用。 在合作营销活动中生成图像的纯文本输出（如副本生成、翻译和品牌对齐建议）不需要C2PA元数据。

## 内容移动时发生的情况 {#cc-content-moves}

同事营销活动会保留与支持的图像资源关联的Content Credentials。 如果导入到同事营销活动中的图像包含Content Credentials，则在生成的营销活动内容和出站电子邮件体验中使用资产时，将保留这些凭据。 [了解有关C2PA元数据的更多信息](https://helpx.adobe.com/cn/firefly/using/content-credentials.html){target="_blank"}。

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

>[!MORELIKETHIS]
>
>[Adobe Experience Cloud Generative AI用户准则](https://www.adobe.com/cn/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}
