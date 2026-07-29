---
title: CX企业应用程序中的AI
description: 了解CX Enterprise应用程序如何使用generative AI (GenAI)、AI Assistant、agentic AI、CX Enterprise Co-worker和MCP工具。
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 870dc2f9f9c13278457248a8db7af3980674efe5
workflow-type: tm+mt
source-wordcount: 872
ht-degree: 2%

---

# CX Enterprise 中的 AI

本指南涵盖Adobe CX Enterprise应用程序中提供的AI功能：用于产品知识和操作见解的创作AI和AI Assistant；用于作业自动化的Agent Orchestrator和Experience Platform Agent；用于实现完全对话的、代理优先体验的CX Enterprise Co-worker；用于将您自己的AI工具连接到CX Enterprise数据的MCP。

## 关于CX Enterprise中的AI

从这里开始，了解在何处以及如何跨CX Enterprise使用AI ：

- [创作AI](./overview/generative-ai.md)介绍了哪些CX Enterprise应用程序支持创作AI和AI Assistant，以及它们之间的比较。
- [代理AI](./overview/agentic-ai.md)说明Experience Platform Agent如何在现有CX Enterprise应用程序和AI优先应用程序中工作，并列出每个应用程序中可用的代理。
- [Agentic AI监控](./overview/monitoring.md)涵盖跟踪代理采用、使用、反馈和AI信用消耗的仪表板。
- [代理作业和AI信用消耗](./overview/ai-credit-consumption.md)说明代理作业如何使用AI信用消耗，并按照代理和作业类型估计消耗率。

## AI 助手

[AI助手](./ai-assistant/ai-assistant-ui.md)是基于Adobe Experience Platform的应用程序中提供的对话式创新型人工智能工具。 使用它获取产品知识、排查问题、查找运营见解和访问Experience Platform代理，所有这些操作都可通过全屏或边栏视图界面中的自然语言提示进行。

阅读[AI助手UI指南](./ai-assistant/ai-assistant-ui.md)以了解如何导航界面，并阅读[提示库](./ai-assistant/prompt-library.md)以了解代理的示例提示。

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

有关代理的完整列表、每个支持的应用程序以及资格要求，请参阅[CX Enterprise中的Agentic AI](./overview/agentic-ai.md)。

## CX Enterprise Co-worker

CX Enterprise Co-worker是AI Assistant的代理优先改进，它自动化了客户体验和营销工作流，因此您的团队可以专注于业务目标而不是例行执行。 您不必一次询问一个问题，而是用自然语言描述一个目标，同事可以计划工作，在您的Adobe和连接的系统中执行工作，验证结果，并返回完成的工作以供您审批。 同事包括：

- **[同事聊天](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/chat/overview)**：用于在CX Enterprise应用程序中浏览数据、验证受众和历程以及完成多步骤任务的对话界面。
- **[同事营销活动](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/campaigns/overview)**：人工智能原生应用程序，使用内置模板、最佳实践和提示性指导，将营销活动简报、受众构建、内容生成、历程设计和校对整合为单一对话体验，以便规模小、敏捷的团队可以快速启动营销活动。
- **同事项目**（即将推出）：用于自动化端到端客户体验编排工作流的统一工作区，帮助团队协调任务、审批和执行以推动从战略到交付的结果。 即将提供项目文档。

符合条件的客户正在逐步从AI助手和Experience Platform代理过渡到同事聊天。 阅读[CX Enterprise Co-worker试用版](./agents/trial.md)以了解试用资格、AI信用使用情况以及如何获得访问权限。

要查看同事聊天的实际效果，请浏览[Playground中的同事聊天](./coworker/playground-coworker-chat.md)，或阅读实际用例，例如[验证AA到CJA的迁移数据](./coworker/data-validation-aa-cja.md)和[分析CJA数据](./coworker/analytics-chat.md)。

有关同事聊天、营销活动和项目的完整产品文档，请参阅[Adobe CX Enterprise同事](./coworker/overview.md)。

## MCP

[Adobe CX Co-worker Gateway](./mcp/overview.md)是CX Enterprise的统一模型上下文协议(MCP)终结点。 它提供与MCP兼容的客户端，如[!DNL Claude]、[!DNL ChatGPT]和[!DNL Cursor]，与您的组织有权使用的产品工具（包括Real-Time CDP、Experience Platform、Journey Optimizer、Customer Journey Analytics和Adobe Analytics）之间的单个受管辖连接。

## 快速入门

### 访问要求

在使用AI助手和Experience Platform代理之前，您的Adobe管理员必须授予相应的权限。 要求因应用程序而异；有关详细信息，请参阅Agent Orchestrator指南中的[访问](./agents/agent-orchestrator.md#access)。

### 隐私和安全性

AI Assistant和Experience Platform代理构建时将隐私、安全和治理放在最前面，包括特定于沙盒的数据隔离和遵循您现有的访问控制策略。 有关完整的详细信息，请阅读[AI助手中的隐私、安全和管理](./ai-assistant/privacy.md)。

## 最佳实践

要从AI助手或同事体验中获得最大价值，请遵循以下最佳实践：

- 在提示中指定&#x200B;**以获取针对性和相关的见解**。
- **通过查看提供的源引用和推理解释来验证响应**。
- **使用上下文设置**&#x200B;以确保您的问题使用了最相关的数据源。
- **提供反馈**&#x200B;以帮助随着时间的推移提高性能和准确性。
- **合并来自多个代理的见解**，以获得更全面的分析。

## 法律注意事项

AI Assistant当前仅支持英语回复，语言模型偶尔可能会出错。 始终验证提供的信息，并使用每个响应中包含的推理步骤来了解信息的生成方式。 有关完整的详细信息，请阅读[法律免责声明](./ai-assistant/legal-disclaimer.md)。

