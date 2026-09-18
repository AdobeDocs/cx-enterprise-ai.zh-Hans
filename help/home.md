---
title: CX Enterprise 应用程序中的 AI
description: 了解CX Enterprise应用程序如何使用创作AI (GenAI)、CX Enterprise Coworker、AI Assistant、代理AI和MCP工具。
TQID: 'https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds'
product_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
    internal-label: CX Enterprise Coworker
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: fccf9111460413fe5b89229564a682827152b1ab
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 2%
---
# CX Enterprise应用程序中的人工智能

本指南介绍Adobe CX Enterprise中的AI功能：创作AI、CX Enterprise Coworker、AI Assistant、Agent Orchestrator和MCP。

## AI功能概述

从这里开始，逐步了解在CX Enterprise中使用人工智能的位置和方式：

- [关于创作AI](./overview/generative-ai.md)介绍了哪些CX Enterprise应用程序支持创作AI和AI助手，以及它们之间的比较情况。
- [关于代理人工智能](./overview/agentic-ai.md)介绍代理人工智能如何在现有CX Enterprise应用程序和AI优先应用程序中工作，并列出每个应用程序中可用的代理。
- [AI监控](./overview/monitoring.md)涵盖跟踪代理采用、使用、反馈和AI信用消耗的仪表板。
- [AI积分消耗](./overview/ai-credit-consumption.md)说明代理作业如何消耗AI积分，并按照代理和作业类型估计消耗率。
- [创作AI内容透明度](./content-transparency.md)介绍Adobe如何跨CX Enterprise应用程序将C2PA元数据自动附加到GenAI生成和GenAI编辑的内容。
- [CX Enterprise代理工具](https://experienceleague.adobe.com/zh-hans/docs/cx-enterprise-agentic-tools/using/overview)涵盖了扩展CX Enterprise代理的其他代理技能和工具（视频教程）。

## Coworker

Co-worker是AI Assistant的代理优先演变，可自动化客户体验和营销工作流，因此您的团队可以专注于业务目标而不是日常执行。 与其一次问一个问题，不如描述一个目标。 同事计划、执行、验证和返回已完成的工作以供您审批。 了解有关[Adobe for Business](https://business.adobe.com/cn/products/cx-enterprise-coworker.html)的更多信息。

同事包括：

- **[同事聊天](https://experienceleague.adobe.com/zh-hans/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/overview)**：用于浏览数据、验证受众和历程以及跨CX Enterprise应用程序完成多步骤任务的对话界面。
- **[团队协作](https://experienceleague.adobe.com/zh-hans/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/overview)**（以前称为&#x200B;_协作营销活动_）：一种AI原生应用程序，可将营销活动简报、受众构建、内容生成、历程设计和校对整合为单一对话体验。 它使用内置模板、最佳实践和提示性指导，帮助小型、敏捷团队快速启动促销活动。 了解有关[Adobe for Business](https://business.adobe.com/cn/products/cx-enterprise-coworker/teams.html)的更多信息。
- **同事项目**（即将推出）：用于自动化端到端客户体验编排工作流的统一工作区，帮助团队协调任务、审批和执行以推动从战略到交付的结果。 即将提供项目文档。

符合条件的客户正在逐步从AI助手和Experience Platform代理过渡到同事聊天。 阅读[同事试用版](./agents/trial.md)以了解试用资格、AI信用使用情况以及如何获取访问权限。

要查看同事聊天的实际效果，请浏览[Playground中的同事聊天](./coworker/playground-coworker-chat.md)，或阅读实际用例，例如[验证AA到CJA的迁移数据](./coworker/chat/use-cases/data-insights/data-validation-aa-cja.md)和[分析CJA数据](./coworker/chat/use-cases/data-insights/analytics-chat.md)。

有关同事聊天、团队和项目的同事的完整产品文档，请参阅[同事](./coworker/overview.md)。 有关沙盒到沙盒对象复制，请参阅[沙盒工具代理技能](./agents/sandbox-tooling.md)。

## AI 助手

[AI助手](./ai-assistant/ai-assistant-ui.md)是基于Adobe Experience Platform的应用程序中提供的对话式创新型人工智能工具。 使用它获取产品知识、排查问题、查找运营见解和访问Experience Platform代理，所有这些操作都可通过全屏或边栏视图界面中的自然语言提示进行。

要了解如何导航界面，请阅读[AI助手用户界面指南](./ai-assistant/ai-assistant-ui.md)。 要查看代理的示例提示，请参阅[提示库](./ai-assistant/prompt-library.md)。

## Agent Orchestrator和Experience Platform代理

[Agent Orchestrator](./agents/agent-orchestrator.md)是支持Experience Platform代理的代理层。 当你向人工智能助手提问时，Agent Orchestrator会规划工作，调用回答问题所需的专业代理，并返回统一的响应，所有这些都由人为监督。

本指南中记录了以下Experience Platform代理：

- [Audience 代理](./agents/audience.md)
- [Data Insights Agent](./agents/cja-data-insights-agent.md)
- [Experimentation Agent](./agents/agent-experiment.md)
- [字段发现代理](./agents/field-discovery-agent.md)
- [Journey Agent](./agents/ajo-agent.md)
- [通知代理](./agents/notifications.md)
- [产品支持代理](./agents/product-support.md)
- [Adobe Marketing Agent for Microsoft 365 Copilot](./agents/ama-ms.md)
- [验证数据](./agents/data-validation.md)

有关代理的完整列表、每个支持的应用程序以及资格要求，请参阅CX Enterprise中的[代理AI](./overview/agentic-ai.md)。

## MCP

[Adobe CX Coworker网关](./mcp/overview.md)是CX Enterprise的统一模型上下文协议(MCP)端点。 它提供了与MCP兼容的客户端，如[!DNL Claude]、[!DNL ChatGPT]和[!DNL Cursor]，与您的组织有权使用的产品工具之间的单个受管辖连接：

- [Real-Time CDP工具](./mcp/rtcdp-mcp.md)
- [Experience Platform工具](./mcp/aep-mcp.md)
- [Journey Optimizer工具](./mcp/ajo-mcp.md)
- [Customer Journey Analytics工具](./mcp/cja-mcp.md)
- [Adobe Analytics工具](./mcp/analytics-mcp.md)
- [!DNL Workfront]工具，记录在[Workfront MCP服务器指南](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/basics/workfront-mcp-server/workfront-mcp-server-overview)中
- [!DNL Target]工具，记录在[目标MCP服务器指南](https://experienceleague.adobe.com/zh-hans/docs/target/using/mcp/target-mcp)中

初次使用CX Coworker Gateway？ 请参阅[访问CX Coworker网关工具](./mcp/access.md)和[安装CX Coworker网关](./mcp/install.md)以连接。 连接后，使用[会话上下文工具](./mcp/context-tools.md)在调用产品工具之前设置活动组织、沙盒和数据视图。

在使用任何这些工具之前，请参阅[开始之前](./overview/overview-ai-cxe.md#before-you-begin)以了解访问要求以及隐私和安全注意事项。

## 最佳实践

要从AI助手或同事体验中获得最大价值，请遵循以下最佳实践：

- 在提示中指定&#x200B;**以获取针对性和相关的见解**。
- **通过查看提供的源引用和推理解释来验证响应**。
- **使用上下文设置**&#x200B;以确保您的问题使用了最相关的数据源。
- **提供反馈**&#x200B;以帮助随着时间的推移提高性能和准确性。
- **合并来自多个代理的见解**，以获得更全面的分析。

## 法律注意事项

AI Assistant目前仅支持英语回复，语言模型偶尔会出错。 始终验证提供的信息，并使用每个响应中包含的推理步骤来了解信息的生成方式。 有关完整的详细信息，请阅读[法律免责声明](./ai-assistant/legal-disclaimer.md)。

Adobe还自动将C2PA元数据附加到跨CX Enterprise应用程序的GenAI生成和GenAI编辑的内容中，以满足创新型人工智能透明度法规。 有关详细信息，请阅读[创作AI内容透明度](./content-transparency.md)。

