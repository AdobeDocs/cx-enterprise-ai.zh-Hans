---
description: 浏览同事聊天用例和示例提示，按区域在数据见解、受众、历程和平台操作之间组织。
title: 同事聊天用例
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 261f478d3dec0845c0a5532201ef6ddc81808372
workflow-type: tm+mt
source-wordcount: 3729
ht-degree: 6%

---

# 同事聊天用例{#use-cases}

Co-worker Chat允许您使用自然语言查询、分析和处理[!DNL Experience Platform]数据，而不是手动导航多个UI或编写查询。 此页面按工作区域整理了从业人员最依赖的用例目录：数据分析、受众、历程、基本元素和沙盒工具。 每个条目都包括它调用的技能、与它一起使用的应用程序以及示例提示，您可以复制、适应自己的数据，并通过对话进行细化。

>[!NOTE]
>
>即将推出：
>
>通过CX Enterprise Co-worker构建的全新AEM代理功能，可帮助您更快完成更多工作。
>
>所有符合条件的客户都可以在Co-worker中以滚动方式访问Adobe Experience Manager代理功能。
>
>另请参阅AEM中的[AI - AEM中的代理功能概述](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/overview)。

## 品牌体验

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 更新AEM页面 | 执行更新、删除、替换或添加内容元素等操作，以保持体验准确且最新。 输入内容可以是自然语言或可视批注，如PDF或屏幕截图。 | `aem-sites-pages-update` | Adobe Experience Manager (AEM) - AEM Sites | 在&lt;URL>上将标题更新为Hello World<br><br>在&lt;URL>上将“参加我们的咖啡测验”按钮更改为更吸引人的版本<br><br>根据附加的<br><br>在&lt;URL>上更新&lt;URL>我想在页面底部添加一个新的Teaser部分，介绍我们在8月份举行的促销活动，购买咖啡机并免费获得2袋咖啡。 还可以找到朋友喝咖啡的图像，并在Teaser中使用 |
| 批量更新AEM | 同时跨多个页面执行批量操作，例如删除、替换或添加内容元素，以保持体验准确且最新。 | `aem-sites-pages-bulkreplace` | Adobe Experience Manager (AEM) - AEM Sites | 在&lt;aem path>上，将包含副本“MyBarista\”的所有页面更新为“BrewPass” |
| 从图转到可视内容片段 | 使用自然语言将设计直接从Figma导入Adobe Experience Manager。 该技能会自动创建所需的内容模型、内容片段、资源和可视化模板，使业务用户能够在几分钟内从设计转移到支持Web的内容，而无需手动设置。 | `aem-sites-visualcontentfragments-create` | Adobe Experience Manager (AEM) - AEM Sites | 从&lt;Figma_URL>导入 |

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 创建表单 | 从纯语言描述、附加的摘要、图像或PDF生成新的自适应表单 | `aem-forms-adaptiveform-create` | Adobe Experience Manager (AEM) - AEM Forms | “创建员工入门培训表单”<br><br>“使用附加的摘要（图像或PDF）创建表单”<br><br>“创建&lt;form type>自适应表单” |
| 编辑/更新表单 | 修改现有表单 — 添加/编辑字段、调整简单布局、配置提交操作或应用附加准则文档的更改 | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) - AEM Forms | “在名字字段下添加中间名字段”<br><br>“将名字和姓氏字段置于2列布局中，50/50”<br><br>“配置表单以将数据发送到REST端点”<br><br>“更新此表单以匹配附加的准则文档”<br><br>“在&lt;现有字段>字段下添加&lt;字段名称>字段” |
| 添加业务逻辑 | 创建简单规则，例如根据其他字段的值显示或隐藏字段 | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) - AEM Forms | “仅在员工类型为承包商时显示‘公司’字段”<br><br>“仅在&lt;其他字段>为&lt;值>时显示&lt;字段>字段” |
| 嵌入表单 | 将现有表单或新创建的表单放置到指定的AEM Sites页面上（仅在Edge Delivery Services页面上受支持） | `aem-forms-adaptiveform-embed` | Adobe Experience Manager (AEM) - AEM Forms | “将此表单嵌入到我们网站的主页上”<br><br>“将此表单嵌入到&lt;页面路径>” |

**相关信息**

* [AEM中的代理功能：Brand Experience - Experience Production - Sites](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-sites)

* [AEM中的代理功能：Brand Experience - Experience Production - Forms](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-forms)

### 开发

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 管理Cloud Manager管道 | 创建、运行和监控AEM Cloud Manager管道，包括日志、工件、变量和设置 | `cloud-manager-pipeline-management` | Adobe Experience Manager (AEM) | “列出项目12345的管道”<br><br>“我最近管道的状态是什么？” |
| 管理Cloud Manager环境 | 创建、配置和维护AEM Cloud Manager环境，包括RDE、环境变量、日志和备份 | `cloud-manager-environment-management` | Adobe Experience Manager (AEM) | 为程序12345列出我的环境&quot;<br><br>&quot;重置我的RDE&quot; |
| 管理Cloud Manager程序 | 列出、检查和删除AEM Cloud Manager程序，包括其管道和环境 | `cloud-manager-program-management` | Adobe Experience Manager (AEM) | “列出我的Cloud Manager程序”<br><br>“获取程序12345的详细信息” |
| 管理AEM版本更新计划 | 为自动维护配置每日免打扰时间和免更新时段，并查看Adobe的全局代码冻结窗口 | `cloud-manager-release-management` | Adobe Experience Manager (AEM) | “我当前的安静时间窗口是什么？”<br><br>“安排12月20日至1月2日的无更新时段” |

**相关信息**

* [AEM中的代理功能：Brand Experience — 开发](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/development/use-cases)

### 入门

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 引导式端到端载入 | 协调完整的入门培训生命周期、存储库选择、文件夹委派、标记、元数据、导入和搜索子技能（如果您不知道需要的特定入门培训任务）。 | `aem-onboarding-workflow` | Adobe Experience Manager (AEM) - AEM Assets | “将我们的团队载入AEM Assets”<br><br>“带我了解AEM DAM载入” |
| 设计和创建文件夹层次结构 | 根据业务需求或CSV输入，在AEM Assets中（在`/content/dam`下）建议和创建可伸缩的文件夹结构。 | `aem-folder-management` | Adobe Experience Manager (AEM) - AEM Assets | “推荐生活方式营销资产的文件夹结构”<br><br>“根据此CSV文件创建文件夹” |
| 设计和创建标记 | 在`/content/cq:tags`下设计和创建受控标记词汇 — 命名空间、分层标记和批量标记操作。 | `aem-tag-taxonomy` | Adobe Experience Manager (AEM) - AEM Assets | “使用产品类别的命名空间设计标记分类”<br><br>“从此CSV导入标记”<br><br>“在AEM中创建这些层次结构标记” |
| 创建和分配元数据表单 | 设计和创建创作UI内容作者使用的自定义元数据表单（从CSV、表、要求文档或描述），然后可以选择将它们分配给文件夹。 | `aem-metadata-form` | Adobe Experience Manager (AEM) - AEM Assets | 从此字段列表创建元数据表单&quot;<br><br>&quot;将此表单分配给`campaigns`文件夹&quot; |

**相关信息**

* [AEM中的代理功能：品牌体验 — 入门](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/onboarding/use-cases)

## 内容审查程序

### 内容发现

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 按语义主题搜索 | 使用AI支持的语义匹配功能，按概念、情绪或视觉主题查找资产。 | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | “给我找一副晨间咖啡生活方式图片” |
| 按自定义元数据搜索 | 按自定义元数据字段筛选资源（例如，Coffee Blend、品牌、Roast级别）。 | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | “查找`Coffee Blend`为`Morning Muse`的资源”<br><br>“获取许可证未过期的资源”<br><br>“查找营销活动名称未设置的资源（必须为属性编制索引以获取相应的结果）。” |
| 按审批状态搜索 | 根据审批状态筛选资源。 例如，已批准、正在审查、已拒绝或缺少状态。 | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | “显示`Campaign`文件夹中所有已批准的资产” |
| 按文件夹/路径搜索 | 通过解释引用AEM中文件夹名称的自然语言提示来识别资源。 您只需在其提示中提及文件夹，而无需手动浏览存储库，即可显着减少找到正确内容所需的点击次数。 | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | “文件夹`WKND`中是否有任何svg”？<br><br>“在文件夹`WKND`中显示在2025年11月1日之后修改的资源” |

**相关信息**

* [AEM中的代理功能：内容顾问 — 内容发现](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/discovery/use-cases)

### 内容优化

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 高分辨率演绎版创建和通道优化的演绎版 | 以指定的分辨率和质量级别生成资产的新演绎版，从而无需手动编辑即可轻松准备渠道就绪的变体。 您还可以根据平台特定要求制作演绎版，如Instagram故事，确保资产自动满足格式、比例和质量准则。 | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | 使用`80% quality`创建`2000px`演绎版作为`JPEG`&quot;<br><br>&quot;为Instagram故事创建演绎版&quot; |
| 标记叠加和复合生成 | 通过精确放置将促销图形、叠加或徽章应用于现有资源，支持快速创建营销活动就绪的合成内容。 | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | “在促销横幅上叠加带有`30%`折扣图表的图像，从中心放置`100px`” |
| 图像增强、背景颜色调整、方向转换 | 应用视觉改进（锐化图像）、替换背景颜色和执行方向转换。 | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | “将`PNG`的背景颜色更改为`#ff8932`”<br><br>“锐化图像”<br><br>“水平镜像图像” |

**相关信息**

* [AEM中的代理功能：内容顾问 — 内容优化](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/content-optimization/use-cases)

## 品牌治理

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 准则和区段查找 | 检索详细的品牌指南，按区段、市场或类别划分范围 | 企业上下文 | Adobe Experience Manager (AEM) | “这个品牌的声调准则是什么？”<br>“列出垂直健康领域使用的索赔类别” |
| 根据品牌指南评估内容 | 根据配置的品牌检查评估已发布/创作的页面、文本块或图像 | aem-governance | Adobe Experience Manager (AEM) | “根据SecurBank准则评估此登陆页面”<br>“此标语是否通过我们的语调检查？” |
| 调试AEM权限 | 调试/了解权限策略、ACL和继承规则。 | aem-governance | Adobe Experience Manager (AEM) | “为什么主体管理员可以在`https://author/`上写`/content/folder/us`？”<br>“为什么无法在`https://author`上的`/content/dam`中采样作者写” |

**相关信息**

* [AEM中的代理功能：品牌管理](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-governance/use-cases)

## 数据分析

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| [提取CJA报告和量度](data-insights/analytics-chat.md) | 实时查询CJA以提取量度、维度、区段和数据视图 | `cja` | Customer Journey Analytics (CJA) | “显示过去30天的页面查看次数”<br>“列出主数据视图中的热门区段” |
| 比较分析 | 并排比较各个渠道、时间段或区段之间的量度 | `cja-root-cause-analysis`, `cja`, `dx-api`, `knowledge-graph` | Customer Journey Analytics (CJA) | “按渠道逐月比较收入”<br>“本季度移动与桌面转化情况如何？” |
| 营销活动效果 | 测量在给定时间段内促销活动、渠道和Web属性的执行情况。 | `cja`, `dx-api`, `knowledge-graph` | | “上个月，我们的Acrobat网络营销活动表现如何？” |
| funnel分析 | 逐步了解每个阶段都存在流失的多步转化漏斗 | `cja` | Customer Journey Analytics (CJA) | &quot;带我浏览funnel&quot; <br> &quot;显示从PDP到购买的转化funnel&quot; |
| 预测 | 基于历史CJA数据预测未来量度值 | `cja` | Customer Journey Analytics (CJA) | “未来30天的预测会话”<br>“我们是否即将实现收入目标？” |
| [根本原因分析](data-insights/root-cause-analysis.md) | 调查量度发生更改的原因：诊断下降、尖峰和异常 | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | “上周为什么转化率下降？” <br> “是什么导致了1月15日的收入激增？” |
| 执行摘要和KPI摘要 | 制作为利益相关者准备的性能摘要、规范性建议和幻灯片组概述 | `cja-executive-summary`, `cja-bacom-anomaly-tracker-v2`, `cja-cno-weekly-pulse`, `cja-reporting`, `cja`, `dx-api` | Customer Journey Analytics (CJA) | “给我上个月的执行摘要”<br>“根据本季度的数据创建一个幻灯片组大纲” |
| [AA ↔ CJA数据验证](data-insights/data-validation-aa-cja.md) | 在Adobe Analytics和Customer Journey Analytics之间比较、审核和协调数据，尤其是在从Adobe Analytics升级到Customer Journey Analytics时 | `aa-cja-validation`, `cja`, `dx-api` | ADOBE ANALYTICS + CJA | “将我的AA报表包与CJA数据视图进行比较”<br>“验证AA和CJA之间的页面视图” |
| 运行时间序列和因果分析 | 查询和分析受众、数据集和具有因果归因的历程的历史时间序列数据 | `operational-stats-causal-analysis` | 所有符合条件的应用程序 | “显示过去90天的受众规模趋势” <br>“为什么我的数据集行数在3月3日激增？” |
| 创建自定义CJA技能 | 将分析模式转变为可重用、可重复的技能，这些技能可在不同会话间持续保留 | `cja-skill-creator` | Customer Journey Analytics (CJA) | “将此每周收入分析转换为可重复使用的技能”<br>“将此技能另存为每月funnel报告的技能” |

## 受众

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| [从自然语言创建受众](audiences/create-audience-from-natural-language.md) | 在每个阶段都通过用户批准来编排受众创建的分步过程 | `audience-creation-flow` | Real-Time CDP (RTCDP) | “创建过去30天内购买的用户受众”<br>“为加利福尼亚州的高价值忠诚度会员构建区段” |
| 构建PQL定义 | 从XDM属性、行为事件或现有受众收集受众定义；支持聚合和时间窗口 | `segment-definition-assembly` | Real-Time CDP (RTCDP) | “为查看了3个以上产品但未购买的用户创建PQL”<br>“向我的事件条件添加7天时间范围” |
| 搜索和查找受众 | 按ID、名称、语义搜索查找受众；检测重复项并分析重叠 | `audience-search` | Real-Time CDP (RTCDP) | “查找所有忠诚受众”<br>“我的‘节假日购物者’区段是否存在重复项？” |
| 估计受众规模 | 使用带有轮询的Adobe Experience Platform预览API估算PQL表达式的配置文件访问范围 | `audience-size-estimate` | Real-Time CDP (RTCDP) | “此受众有多大？”<br> “此PQL表达式的预计范围” |
| 受众规模瀑布 | 将PQL分解为子谓词，并显示每个条件对最终受众规模的贡献 | `audience-size-waterfall` | Real-Time CDP (RTCDP) | “向我显示此PQL的瀑布图”<br>“细分每个条件如何减少受众” |
| 发现用于定位的XDM字段 | 按名称、描述或数据值搜索字段；查看字段的生活位置和使用位置 | `field-discovery` | Real-Time CDP (RTCDP) | “我可以使用哪些字段来定位忠诚度客户？”<br> “查找与购买历史记录相关的字段” |
| 发布/保存受众 | 通过命名约定和合规性检查将受众定义保留到Experience Platform分段服务 | `audience-publish` | Real-Time CDP (RTCDP) | “将此内容另存为草稿”<br>“发布名称为‘春季促销买家’的受众” |

## 历程

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| [从自然语言创建历程](journeys/create-journey-from-natural-language.md) | 在AJO中通过文本提示或上传的图像/流程图编排旅程创建 | `journey-create` | Adobe Journey Optimizer (AJO) | “创建一个欢迎历程，注册后发送电子邮件，等待3天，然后发送跟进”<br>“从此上传的流程图图像构建历程” |
| 分析历程冲突 | 检测活动历程之间的受众重叠、计划冲突和重复数据删除问题 | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | “我的购物车放弃历程是否与任何其他历程冲突？” <br> “检查我的活动历程之间的受众重叠” |
| 分析历程流失 | 识别客户在旅程中的流失位置和原因，并检测导致脱离接触的行为模式 | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | “在我的重新参与历程中，客户从哪里流失？”<br> “历程X中的哪些节点的流失率最高？” |
| 分析自定义操作错误 | 识别历程中自定义操作何时失败或错误率激增，并在故障升级为更广泛中断之前诊断根本原因 | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | “为什么自定义操作在我的忠诚度注册历程中失败？” <br> “在我的欢迎历程中向我显示自定义操作ExternalPush的错误率。” |
| [创建、编辑和管理忠诚度挑战](journeys/create-loyalty-challenge.md) | 简化并加快忠诚度计划管理 | `loyalty` | Adobe Journey Optimizer (AJO) | “创建挑战，鼓励会员尝试新的季节性饮品”<br>“向我展示会员流失率最高的忠诚度挑战。” |

## 基本元素

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 产品知识和文档 | 从官方Adobe文档中回答操作方法、概念、故障排除和最佳实践问题 | `product-knowledge` | 所有符合条件的应用程序 | “如何设置流目标？”<br> “批量分段与流式分段之间有何区别？” |
| 查询Experience Platform/Journey Optimizer实体 | 作为有关平台实体的问题的主要入口点；根据需要路由到KG 、字段发现或API | `operational-insights` | 所有符合条件的应用程序 | “我有多少数据集？” <br> “显示所有活动的历程”<br>“列出我的目标” |
| 知识图查询 | 通过单个SQL查询进行聚合计数、跨实体联接、关系查找和元数据探索 | `knowledge-graph` | 所有符合条件的应用程序 | “哪些受众使用此数据集？”<br> &quot;向我显示架构和数据集之间的关系&quot; |
| Experience Platform / Journey Optimizer / Customer Journey Analytics API操作 | 提供直接API网关，用于处理知识图中没有的突变、实时状态检查和实体类型 | `cxo-api` | 所有符合条件的应用程序 | “删除数据集X”<br>“检查我的批次摄取作业的状态” |
| 实体解析和链接 | 使用语义和词法搜索将实体提及解析为实际的Experience Platform实体并发现XDM字段 | `entity-linking` | Adobe Experience Platform | “将‘假日购物者’解析为实际受众”<br>“查找与购买历史记录相关的字段” |
| 管理自定义技能 | 保存、修改或删除跨会话保留的用户拥有的可重用技能 | `manage-skill` | 所有符合条件的应用程序 | “将该工作流另存为技能” <br>“删除我的每周报告技能” <br>“将此技能转换为可重复使用的技能” |
| 监控流容量和违规情况 | 检查沙盒中的当前和历史流使用情况、容量和违规状态 | `observability-streaming-capacity`, `observability-streaming-usage`, `observability-capacity-breaches` | Adobe Experience Platform | “我的当前沙盒中的当前流容量是多少？” <br> “我当前的沙盒在上周是否超出了容量限制？” |
| [查看运行状况检查评估结果](https://experienceleague.adobe.com/en/docs/experience-platform/run-and-operate/health-checks/overview) | 查看沙盒的最新运行状况检查评估，深入研究未通过检查，并查看受影响的实体 | `rao-view-latest-health-checks-assessment` | Adobe Experience Platform | “我的沙盒有什么问题？” <br> “告诉我关于我最新的运行状况检查评估的信息” <br> “自定义命名空间描述检查有哪些问题？” |
| 修复运行状况检查问题 | 在进行任何更改之前，经您批准，可直接从聊天中修复标记的身份命名空间、合并策略和架构问题 | `rao-remediate-identity-namespace-description`, `rao-remediate-merge-policy-duplicate-name`, `rao-remediate-missing-audit-field-group`, `rao-remediate-default-merge-policy-naming` | Adobe Experience Platform | “修复身份命名空间描述”<br>“修复重复的合并策略名称”<br>“修复缺少审核字段组的架构”<br>“修复默认合并策略命名” |

## 沙盒工具

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| [跨沙盒移动对象](/help/agents/sandbox-tooling.md) | 通过自动解析依赖关系，跨沙盒无缝迁移架构、受众和其他对象配置 | `sandbox-tooling-workflow` | Adobe Experience Platform | “将架构Luma忠诚度会员白金从当前沙盒移动到生产沙盒”<br>“将美国黄金忠诚度会员受众提升到暂存环境” |

## 客户警报

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 管理警报订阅 | 通过自然语言对话查看和管理警报订阅。 | `alerts-subscribe` | Adobe Experience Platform | “我订阅了哪些警报？”<br><br>“为我订阅此警报。”<br><br>“删除此警报的订阅。” |
| 查看警报活动 | 查看指定时间段内的当前警报状态和历史警报活动。 | `alerts-list` | Adobe Experience Platform | “过去24小时内发生了什么？”<br><br>“过去24小时内触发了哪些警报？”<br><br>“显示过去七天的活动警报。” |
| 识别定期警报模式 | 分析警报历史记录，以识别频繁触发的警报类型和操作趋势。 | `alerts-list` | Adobe Experience Platform | “显示前3个触发的警报类型。”<br><br>“哪些警报类型本月发生得最频繁？”<br><br>“您最近七天看到了哪些警报模式？” |
| 关注高度优先的问题 | 按严重程度筛选警报活动以安排调查工作的优先级。 | `alerts-list` | Adobe Experience Platform | “仅显示高严重性警报。”<br><br>“本周触发了哪些严重性警报？”<br><br>“显示过去30天的严重性警报。” |
| 了解警报的影响范围 | 确定受警报影响最大的对象并确定应从何处开始调查。 | `alerts-list` | Adobe Experience Platform | “前5个受影响的对象是什么？”<br><br>“哪些对象与最高级别警报关联？” |
| 将警报类型连接到受影响的对象 | 分析警报类型和受影响资源之间的关系。 | `alerts-list` | Adobe Experience Platform | “哪些警报类型最常影响此数据集？”<br><br>“显示警报类型与受影响对象之间的关系。”<br><br>“哪些警报类型最常影响最受影响的对象？” |
| 关注我的警报 | 分析您订阅并负责监视的警报。 | `alerts-list` | Adobe Experience Platform | “显示我订阅的高严重性警报。”<br><br>“本周触发了来自我的警报的哪些警报？”<br><br>“我的任何订阅警报需要关注吗？” |

## 工作流和规划

| 用例 | 描述 | 技能 | 应用程序 | 示例提示 |
| --- | --- | --- | --- | --- |
| 管理规划工作区 | 构建和改进Workfront Planning工作区、部分、记录类型和字段，以组织项目和跟踪工作 | `manage-workfront-planning`, `wf-planning-solution-architect` | Workfront规划 | “创建一个名为MKG Hub的工作区并设置记录类型以按地区跟踪程序”<br>“设置跨渠道和区域跟踪MKG程序所需的记录类型和关系” |
| 管理规划记录 | 在工作区中创建和更新规划记录（营销活动、摘要）及其字段值 | `manage-workfront-planning` | Workfront规划 | “为秋季品牌发布活动创建简报，包括目标、目标受众和关键消息”<br>“使用预算和主要渠道更新秋季品牌发布简报” |
| 创建和管理项目 | 启动和构建项目 — 应用模板、设置优先级和预算、对任务进行排序、添加阶段和依赖项以及分配人员或角色 | `manage-workfront-workflow` | Workfront工作流程 | “创建春季营销活动，用$200K预算将其设置为高优先级，然后排列任务顺序” <br> “从[项目模板]创建名为[项目名称]的Workfront项目计划” <br> “为秋季发布活动构建项目计划 — 社交营销活动，包含概念、设计、复制和审阅任务” <br> “添加新电子邮件营销任务并将其分配给Rachel Smith” |
| 加快审查和批准 | 设置多阶段批准、应用批准模板、添加/删除批准者、发送提醒并进行批量更新 | `manage-workfront-workflow` | Workfront工作流程 | “创建多阶段审批 — 复制、设计、法律 — 并提醒未批准的人”<br>“将Chris Smith从所有未完成的审批中移除，并替换为Jane Francis” |
| 更新任务和工作状态 | 标记任务完成、更新完成百分比并关闭您的工作 | `manage-workfront-workflow` | Workfront工作流程 | “将我在秋季启动项中的‘生成关键艺术’任务标记为完成”<br>“100%关闭我的秋季启动项复制任务” |
| 表面工作分析 | 提出探索性问题以查找存在风险的工作、未分配任务、未完成的问题和跨项目的状态 | `query-workfront` | Workfront工作流程 | “查找未分配给任何人和本周到期的当前项目中的未完成任务”<br>“当前项目中有多少个未完成的问题？” |
| 项目和任务摘要 | 项目、任务、问题和分配的拉取列表、表和计数 | `query-workfront` | Workfront工作流程 | “显示已准备开始的任务的表，其中具有项目名称、任务到期日期和分配的用户”<br>“获取分配给[用户名]的所有任务” |
| 跟踪批准和项目组合状态 | 检查审批状态，并按项目组合汇总未完成的工作 | `query-workfront` | Workfront工作流程 | “显示我的审批状态”<br>“显示包含未完成问题的表，这些问题是[Portfolio名称]项目组合的一部分” |
