---
description: 浏览同事聊天用例和示例提示，按区域在数据见解、受众、历程和平台操作之间组织。
title: 用例
source-git-commit: ca4515cb9010fb352489700108bbfe95396b0ad3
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 3%

---

# 用例 {#use-cases}

下面是从业人员在Adobe CX Enterprise Co-worker Chat中使用的用例和示例提示，按工作区组织。 每个提示都构建为可复制、根据您自己的数据和上下文进行调整，并通过对话进行细化。

## 数据分析

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 提取CJA报表和量度 | 实时查询CJA以提取量度、维度、区段和数据视图 | `cja` | Customer Journey Analytics (CJA) | “显示过去30天的页面查看次数” · “在主数据视图中列出排名最前的区段” |
| 比较分析 | 并排比较各个渠道、时间段或区段之间的量度 | `cja` | Customer Journey Analytics (CJA) | “按渠道逐月比较收入” · “本季度移动设备与台式机转化情况如何？” |
| funnel分析 | 逐步了解每个阶段都存在流失的多步转化漏斗 | `cja` | Customer Journey Analytics (CJA) | &quot;带我浏览funnel结账&quot; · &quot;显示从PDP到购买的转化funnel&quot; |
| 预测 | 基于历史CJA数据预测未来量度值 | `cja` | Customer Journey Analytics (CJA) | “未来30天的预测会议” · “我们是否即将实现收入目标？” |
| 根本原因分析 | 调查量度发生更改的原因：诊断下降、尖峰和异常 | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | “为什么上周的转化率下降了？” · “是什么导致1月15日收入激增？” |
| 执行摘要和KPI摘要 | 制作为利益相关者准备的性能摘要、规范性建议和幻灯片组概述 | `cja-executive-summary` | Customer Journey Analytics (CJA) | “给我上个月的执行摘要” · “根据本季度的数据创建一个幻灯片组大纲” |
| AA ↔ CJA数据验证 | 在Adobe Analytics和Customer Journey Analytics之间比较、审核和协调数据 | `aa-cja-validation` | ADOBE ANALYTICS + CJA | “将我的AA报表包与CJA数据视图进行比较” · “验证AA和CJA之间的页面视图” |
| 运行时间序列和因果分析 | 查询和分析受众、数据集和具有因果归因的历程的历史时间序列数据 | `operational-stats-causal-analysis` | 所有符合条件的应用程序 | “显示过去90天的受众规模趋势” · “为什么我的数据集行数在3月3日激增？” |
| 创建自定义CJA技能 | 将分析模式转变为可重用、可重复的技能，这些技能可在不同会话间持续保留 | `cja-skill-creator` | Customer Journey Analytics (CJA) | “将此每周收入分析转换为可重复使用的技能” · “将此技能另存为每月funnel报告的技能” |

## 受众

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 从自然语言创建受众 | 在每个阶段都通过用户批准来编排受众创建的分步过程 | `audience-creation-flow` | Real-Time CDP (RTCDP) | “创建过去30天内购买的用户受众” · “在加利福尼亚为高价值忠诚度会员构建区段” |
| 构建PQL定义 | 从XDM属性、行为事件或现有受众收集受众定义；支持聚合和时间窗口 | `segment-definition-assembly` | Real-Time CDP (RTCDP) | “为查看了3个以上产品但未购买的用户创建PQL” · “向我的事件条件添加7天时间范围” |
| 搜索和查找受众 | 按ID、名称、语义搜索查找受众；检测重复项并分析重叠 | `audience-search` | Real-Time CDP (RTCDP) | “查找所有忠诚受众” · “我的‘节日购物者’区段是否存在重复项？” |
| 估计受众规模 | 使用带有轮询的AEP预览API估算PQL表达式的配置文件访问范围 | `audience-size-estimate` | Real-Time CDP (RTCDP) | “这些受众有多大？” · “估算此PQL表达式的范围” |
| 受众规模瀑布 | 将PQL分解为子谓词，并显示每个条件对最终受众规模的贡献 | `audience-size-waterfall` | Real-Time CDP (RTCDP) | “向我展示此PQL的瀑布图” · “划分每个条件如何减少受众” |
| 发现用于定位的XDM字段 | 按名称、描述或数据值搜索字段；查看字段的生活位置和使用位置 | `field-discovery` | Real-Time CDP (RTCDP) | “可使用哪些字段来定位忠诚客户？” · “查找与购买历史记录相关的字段” |
| 发布/保存受众 | 通过命名约定和合规性检查将受众定义保留到AEP分段服务 | `audience-publish` | Real-Time CDP (RTCDP) | “保存为草稿” · “发布名称为‘春季促销买家’的受众” |

## 历程

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 从自然语言创建历程 | 在AJO中通过文本提示或上传的图像/流程图编排旅程创建 | `journey-create` | Adobe Journey Optimizer (AJO) | “创建一个欢迎历程，在注册后发送电子邮件，等待3天，然后发送跟进” · “从此上传的流程图图像构建历程” |
| 分析历程冲突 | 检测活动历程之间的受众重叠、计划冲突和重复数据删除问题 | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | “我的购物车放弃历程是否与其他历程冲突？” · “检查我的活动历程之间的受众重叠” |
| 分析历程流失 | 识别客户在旅程中的流失位置和原因，并检测导致脱离接触的行为模式 | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | “在我的重新参与之旅中，人们会在哪里掉头？” · “历程X中的哪些节点的流失率最高？” |
| 分析自定义操作错误 | 识别历程中自定义操作何时失败或错误率激增，并在故障升级为更广泛中断之前诊断根本原因 | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | “为什么自定义操作在我的忠诚度注册历程中失败？” · “在我的欢迎历程中向我显示自定义操作ExternalPush的错误率。” |

## 基本元素

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 产品知识和文档 | 从官方Adobe文档中回答操作方法、概念、故障排除和最佳实践问题 | `product-knowledge` | 所有符合条件的应用程序 | “如何设置流目标？” · “批量分段与流式分段之间有何区别？” |
| 查询AEP/AJO实体 | 作为有关平台实体的问题的主要入口点；根据需要路由到KG 、字段发现或API | `operational-insights` | 所有符合条件的应用程序 | “我有多少数据集？” · “显示所有活动的历程” · “列出我的目标” |
| 知识图查询 | 通过单个SQL查询进行聚合计数、跨实体联接、关系查找和元数据探索 | `knowledge-graph` | 所有符合条件的应用程序 | “哪些受众使用此数据集？” · “向我显示架构和数据集之间的关系” |
| AEP/AJO/CJA API操作 | 提供直接API网关，用于处理知识图中没有的突变、实时状态检查和实体类型 | `cxo-api` | 所有符合条件的应用程序 | &quot;删除数据集X&quot; · &quot;检查我的批量摄取作业的状态&quot; |
| 实体解析和链接 | 使用语义和词法搜索将实体提及解析为实际的AEP实体并发现XDM字段 | `entity-linking` | Adobe Experience Platform (AEP) | “将‘假日购物者’解析为实际受众”·“查找与购买历史记录相关的字段” |
| 构建个人上下文 | 从AEP、CJA和/或Workfront活动日志生成个性化的用户配置文件 | `build-my-context` | 所有符合条件的应用程序 | “从AEP和CJA活动构建我的上下文”· “我在此组织中是谁？” |
| 提取组织上下文 | 将文档中的组织范围知识提取到共享的组织上下文Wiki中 | `distill-org-context` | 所有符合条件的应用程序 | “将此文档提取到组织wiki”·“将此文件添加到组织上下文” |
| 提取用户上下文 | 将个人工作上下文从文档提取到用户上下文Wiki中 | `distill-user-context` | 所有符合条件的应用程序 | “将此文件添加到我的用户上下文”·“从此文档中提取我的工作上下文” |
| 管理自定义技能 | 保存、修改或删除跨会话保留的用户拥有的可重用技能 | `manage-skill` | 所有符合条件的应用程序 | 将工作流另存为技能” · “删除我的每周报告技能” · “将此转换为可重复使用的技能” |

## 沙盒工具

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 跨沙盒移动对象元数据 | 通过自动解析依赖关系，跨沙盒无缝迁移架构、受众和其他对象配置 | `sandbox-tooling-workflow` | Adobe Experience Platform (AEP) | “将架构Luma忠诚会员白金从当前沙盒移动到生产沙盒”· “将美国金牌忠诚会员受众提升到暂存环境” |
