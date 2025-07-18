# Amazon Bedrock AgentCore Runtime

## 概述
Amazon Bedrock AgentCore Runtime 是一种安全、无服务器的运行时，专为部署和扩展 AI 代理和工具而设计。
它支持任何框架、模型和协议，使开发人员能够以最少的代码更改将本地原型转变为生产就绪的解决方案。

Amazon BedrockAgentCore Python SDK 提供了一个轻量级包装器，帮助您将代理函数部署为与 Amazon Bedrock 兼容的 HTTP 服务。它处理所有 HTTP 服务器细节，使您可以专注于代理的核心功能。

您只需要使用 `@app.entrypoint` 装饰器装饰您的函数，并使用 SDK 的 `configure` 和 `launch` 功能将您的代理部署到 AgentCore Runtime。然后，您的应用程序可以使用 SDK 或任何 AWS 开发者工具（如 boto3、AWS SDK for JavaScript 或 AWS SDK for Java）调用此代理。

![Runtime 概述](images/runtime_overview.png)

## 主要特点

### 框架和模型灵活性

- 从任何框架（如 Strands Agents、LangChain、LangGraph、CrewAI）部署代理和工具
- 使用任何模型（无论是否在 Amazon Bedrock 中）

### 集成

Amazon Bedrock AgentCore Runtime 通过统一的 SDK 与其他 Amazon Bedrock AgentCore 功能集成，包括：

- Amazon Bedrock AgentCore Memory
- Amazon Bedrock AgentCore Gateway
- Amazon Bedrock AgentCore Observability
- Amazon Bedrock AgentCore Tools

这种集成旨在简化开发过程，并为构建、部署和管理 AI 代理提供全面的平台。

### 使用场景

该运行时适用于广泛的应用，包括：

- 实时、交互式 AI 代理
- 长时间运行的复杂 AI 工作流
- 多模态 AI 处理（文本、图像、音频、视频）

## 教程概述

在这些教程中，我们将涵盖以下功能：

- [托管代理](01-hosting-agent)
- [托管 MCP 服务器](02-hosting-MCP-server)
- [高级概念](03-advanced-concepts)