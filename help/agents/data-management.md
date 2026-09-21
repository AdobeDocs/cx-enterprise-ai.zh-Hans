---
title: Adobe Experience Platform数据管理代理
description: 了解如何使用CX Coworker中的数据管理代理查找和分析Adobe Experience Platform数据集，并管理数据湖保留策略。
source-git-commit: 40f144c7a06592c78dccc6c17f19554b62f667c9
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 3%
---
# 数据管理代理

>[!AVAILABILITY]
>
>数据管理代理可供所有有权访问Adobe CX Enterprise Coworker的客户使用。

要了解和管理Experience Event数据集的数据湖保留，请使用CX Coworker中的Data Management Agent。 随着Adobe Experience Platform数据湖中的体验事件数据集的增长，完成查询和下游流程可能需要更长时间，同时保留要求也变得更加难以管理。 用自然语言描述您想要完成的任务。 Data Management Agent可查找相关的Experience Event数据集，分析这些数据集的使用积极性，并模拟建议的保留期将影响的数据量。 当您准备好采取行动时，它可帮助您设置、更改或删除保留策略，并在进行任何更改之前要求您确认。

## 数据管理代理可以执行的操作 {#what-the-data-management-agent-can-do}

Data Management Agent提供四种技能。

>[!NOTE]
>
>列出数据集、分析数据集使用情况和分析数据集保留技能均为只读。 只有“管理数据集保留”技能才能更改数据湖保留策略，并且在应用任何更改之前需要您明确确认。

| 技能 | 描述 |
|---|---|
| **列出数据集** | 在决定从何处开始保留审查时使用。 列出具有存储大小、行数、现有保留设置和配置文件启用的体验事件数据集，以便快速识别可能适合数据湖保留策略的数据集 |
| **分析数据集使用情况** | 在决定数据集是否是数据湖保留策略的良好候选数据集之前使用。 根据信号（如最近的摄取、查询活动和下游应用程序使用情况）对特定数据集的使用方式进行分类。 |
| **分析数据集保留** | 在提交到保留期之前使用。 显示数据集的存储量度及其数据的年龄，然后使用该年龄分布来估计潜在保留期将保留或删除的数据量。 |
| **管理数据集保留** | 在您准备好采取行动时使用。 设置、更改或删除数据集上的数据湖保留策略，并在进行任何更改之前进行影响预览和确认。 |

## 范围：数据湖保留与其他数据管理工具 {#scope}

在需要查找和分析Experience Event数据集以及设置、更改或删除数据湖保留策略时，请使用数据管理代理。

如果您不确定数据湖保留策略是否是您目标的正确选项，请参阅[选择正确的数据生命周期管理功能](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-lifecycle/choose-a-capability)，以比较可用的保留和删除选项。

这些技能不会管理以下相关功能：

- **配置文件存储保留策略。** 要管理体验事件在配置文件存储中保留的时长，请在启用配置文件的体验事件数据集上配置体验事件过期策略。 请参阅[体验事件过期](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/profile/event-expirations)。
- **沙盒范围的假名配置文件数据过期。** 要在沙盒满足配置的条件后自动删除假名配置文件数据，请参阅[假名配置文件](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/profile/pseudonymous-profiles)。
- **数据集过期。** 要计划在未来日期删除整个数据集，请参阅[数据集过期](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-lifecycle/ui/dataset-expiration)。
- **记录删除。** 若要出于隐私或卫生原因删除个人配置文件记录，请参阅[记录删除](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-lifecycle/ui/record-delete)。

## 先决条件 {#prerequisites}

在开始之前，请确保您具有：

- 访问Adobe Experience Platform以及包含要审查的数据集的沙盒。
- 您需要使用的数据集和保留操作所需的Adobe Experience Platform权限。 Data Management Agent使用您现有的Experience Platform权限，不授予其他访问权限。 有关Adobe Experience Platform权限和角色的工作方式，请参阅[访问控制概述](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/access-control/home)。
- CX Coworker中安装的Adobe CXO插件。

有关安装插件的说明，请参阅[辅助进程UI指南](https://experienceleague.adobe.com/zh-hans/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide)。

## 使用数据管理代理 {#use-the-data-management-agent}

使用自然语言通过CX Coworker与Data Management Agent交互。 描述您的目标，然后通过后续问题优化结果。

>[!NOTE]
>
>在开始之前，请确保您使用的是包含要审阅的数据集的沙盒。

要使用数据管理代理，请执行以下操作：

1. 导航到&#x200B;**[!UICONTROL CX Coworker]**。 有关访问详细信息，请参阅[辅助进程UI指南](https://experienceleague.adobe.com/zh-hans/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide)。
1. 输入说明要完成的任务的要求。
1. 检查结果并使用跟进问题继续调查。

如果请求更改了数据湖保留策略，Data Management Agent将显示建议的影响，并需要在应用更改之前进行确认。

有关用于识别数据集、分析使用情况和保留影响以及管理数据湖保留策略的端到端工作流，请参阅[管理数据湖保留](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md)。

## Data Management Agent的工作原理 {#how-the-data-management-agent-works}

数据管理代理使用确定性计算来分析数据集使用情况，因此相同的输入将生成相同的使用层。 它还以编程方式计算维系率影响，而不是依赖人工智能生成的估计值。 保留影响仍是一种近似值，因为它基于数据的年龄分布。 代理直接从Adobe Experience Platform服务中检索数据，以提供有关数据集的当前信息。

## 限制 {#limitations}

数据管理代理可以识别可能是数据湖保留策略的良好候选数据集，但它不会决定某个数据集是否需要该数据集。 未经您明确确认，它不会应用、更改或删除保留策略。

## 后续步骤 {#next-steps}

有关使用每种技能在体验事件数据集上查找、分析和管理数据湖保留的指导，请参阅[管理数据湖保留](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md)。

有关数据湖保留策略在Adobe Experience Platform中如何工作的更多信息，包括保留行为和配置，请参阅[Experience Event数据集保留(TTL)指南](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/catalog/datasets/experience-event-dataset-retention-ttl-guide)。
