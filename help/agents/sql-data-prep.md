---
title: Co-worker中的SQL数据准备
description: 了解如何在Co-worker中使用SQL数据准备来生成、优化、排查和计划SQL查询。
source-git-commit: dff76b520c013554276e72a3e19b5d56c16af5fa
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 1%
---
# Co-worker中的SQL数据准备

在Co-worker中使用SQL数据准备来执行带有自然语言提示的常用[数据Distiller](https://experienceleague.adobe.com/en/docs/experience-platform/query/data-distiller/overview)任务。 您可以生成SQL、对现有查询进行故障诊断或优化、预览结果，以及计划定期执行的查询。

>[!AVAILABILITY]
>
>在Co-worker中准备的SQL数据在Limited Availability中提供。

## 先决条件 {#prerequisites}

在Co-worker中使用SQL数据准备之前，请确保您具有：

- 数据Distiller权利。
- 访问同事。

## 快速入门 {#get-started}

要开始，请打开Co-worker并输入描述要实现的SQL任务或结果的自然语言请求。

您可以确定要在请求中使用的数据集。 如果需要其他信息才能完成任务，同事可以在继续之前询问后续问题。

Co-worker生成或更新SQL后，您可以继续对话以预览结果、优化查询、保存查询或安排其定期执行。

有关使用同事界面的指导，请参阅[同事用户界面指南](../coworker/chat/ui-guide.md)。

## 支持的功能 {#supported-capabilities}

可以将SQL数据准备用于以下任务：

| 功能 | 描述 |
| --- | --- |
| **SQL创作** | 根据要执行的数据操作的自然语言描述生成SQL。 |
| **SQL优化** | 分析现有Data Distiller查询并优化其性能，同时保留其预期结果。 |
| **SQL错误诊断和更正** | 诊断现有SQL查询中的错误，说明根本原因，并生成已更正的SQL。 |
| **查询计划和警报** | 保存和计划定期执行的查询，并配置支持的查询警报。 |

## 在对话中使用SQL数据准备 {#work-with-sql-data-preparation}

您可以将SQL数据准备功能合并到同一同事对话中，而不是将它们视为单独的工作流。

例如，您可以：

1. 描述所需的结果并生成SQL。
2. 预览最多五行的查询结果。
3. 优化查询或询问有关生成的SQL的问题。
4. 保存查询。
5. 计划定期执行的查询并配置警报。

在需要其他信息时，同事可以询问跟进问题，例如确定合适的数据集或确认时间表的时区。

查询预览最多返回五行。 要直接在Experience Platform中运行和使用查询，请参阅[查询编辑器UI指南](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/user-guide)。

![Co-worker响应显示SQL查询结果的五行预览，以及用于将查询另存为模板或计划其定期执行的选项。](./assets/sql-data-prep/query-preview.png)

### 从自然语言生成SQL {#generate-sql}

如果您知道要实现的结果或转换，但希望Co-worker生成相应的SQL，请使用SQL创作。

为了从正确的数据生成SQL，Co-worker可以识别和验证涉及的数据集。 如果您的请求未提供足够的信息来确定合适的数据集，同事可以在继续之前提出后续问题。

例如：

> 嗨！ 使用test_luma_web_events_1000，按事件类型汇总客户参与情况。 显示事件类型、事件总数和独特客户。 每个事件类型返回一行，并按独特客户从高到低对结果进行排序。

Co-worker会返回生成的SQL，并且可以执行查询以提供结果的预览。

![Co-worker响应显示按事件类型汇总客户参与情况的已生成SQL，随后是事件总数和独特客户的表预览以及结果分析。](./assets/sql-data-prep/authoring-result.png)

有关直接在Experience Platform中创建和运行查询的信息，请参阅[查询编辑器用户界面指南](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/user-guide)。

### 优化现有SQL {#optimize-sql}

当您已经拥有Data Distiller查询并希望在不更改其预期结果的情况下提高其性能时，请使用SQL优化。

您可以要求同事解释更改，比较原始和优化的SQL，并提供验证或查询计划信息。

例如：

> 针对数据Distiller性能优化以下查询，同时保留完全相同的结果。 解释您更改了什么以及优化查询在逻辑上等价的原因。
>
> ```sql
> SELECT
>         p.customer_id,
>         p.first_name,
>         p.last_name,
>         p.loyalty_status,
>         COUNT(o.order_id) AS total_orders,
>         SUM(CAST(o.order_total AS DOUBLE)) AS total_revenue
> FROM test_luma_profiles_1000 p
> INNER JOIN test_luma_orders_1000 o
>         ON p.customer_id = o.customer_id
> GROUP BY
>         p.customer_id,
>         p.first_name,
>         p.last_name,
>         p.loyalty_status
> ORDER BY total_revenue DESC;
> ```
>
> 向我发送完整的响应，特别是原始SQL、优化的SQL、等效性说明以及任何EXPLAIN/验证结果。

如果提供的查询已优化，同事可以确定不需要修改，并解释其评估。

![同事响应正在分析现有SQL查询以进行优化并解释不需要更改，同时具有查询计划发现结果和等效评估。](./assets/sql-data-prep/optimize-query.png)

已优化通过SQL创作功能生成的SQL。 您无需单独提交新生成的SQL以进行优化。

有关SQL语法和支持的命令，请参阅[查询服务SQL引用](https://experienceleague.adobe.com/en/docs/experience-platform/query/sql/overview)。

### 诊断和修复SQL错误 {#diagnose-sql-errors}

当现有查询失败并且您需要帮助确定原因和纠正SQL时，请使用SQL错误诊断。

Co-worker分析查询，确定错误原因，解释问题并提供更正后的SQL。

例如：

> 嗨！ 以下查询失败。 诊断错误，解释根本原因，并提供正确的查询：
>
> ```sql
> SELECT
>         o.order_id,
>         o.product_id,
>         p.product_name,
>         o.order_total
> FROM test_luma_orders_1000 o
> JOIN test_luma_product_catalog_1000 p
>         ON o.productid = p.productid;
> ```
>
> 更正后的查询应使用来自两个数据集的相应产品ID字段。

更正查询后，您可以要求同事执行查询并预览结果。

![Co-worker响应诊断因产品ID字段名称不正确导致的SQL查询错误，并提供使用product_id字段的更正SQL。](./assets/sql-data-prep/diagnose-error.png)

### 计划查询和配置警报 {#schedule-queries}

生成、更正或预览查询后，您可以继续对话以保存并计划定期执行。

例如：

> 将此查询安排在每天早上6:00运行。 配置查询失败时的警报。

如果所需信息缺失或不明确，同事会在创建时间表之前询问后续问题。 例如，它可以要求您确认与请求的执行时间关联的时区。

确认所需的计划详细信息后，Co-worker会返回已保存查询模板、计划、时区、状态和失败警报的汇总。

![确认计划SQL查询的同事响应，包括保存的模板、计划、时区、结束日期、计划状态和失败警报。](./assets/sql-data-prep/schedule-query.png)

有关查询计划、循环设置、输出数据集和警报的详细信息，请参阅[查询计划](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/query-schedules)。

## 后续步骤 {#next-steps}

有关SQL数据准备使用的数据Distiller和查询服务功能的更多信息，请参阅以下文档：

- [数据Distiller概述](https://experienceleague.adobe.com/en/docs/experience-platform/query/data-distiller/overview)
- [查询编辑器UI指南](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/user-guide)
- [查询计划](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/query-schedules)
- [查询服务SQL引用](https://experienceleague.adobe.com/en/docs/experience-platform/query/sql/overview)
