# 在 Amazon Bedrock AgentCore Runtime 中托管使用 OpenAI 模型的 Strands Agents

## 概述

在本教程中，我们将学习如何使用 Amazon Bedrock AgentCore Runtime 托管您现有的代理。

我们将重点关注使用 OpenAI 模型的 Strands Agents 示例。有关使用 Amazon Bedrock 模型的 Strands Agents 示例，请查看[这里](../01-strands-with-bedrock-model)，
有关使用 Amazon Bedrock 模型的 LangGraph 示例，请查看[这里](../02-langgraph-with-bedrock-model)。


### 教程详情

| 信息             | 详情                                                                  |
|:--------------------|:-------------------------------------------------------------------------|
| 教程类型       | 对话式                                                           |
| 代理类型          | 单一                                                                   |
| 代理框架   | Strands Agents                                                           |
| LLM 模型           | GPT 4.1 mini                                                             |
| 教程组件 | 在 AgentCore Runtime 上托管代理。使用 Strands Agent 和 OpenAI 模型 |
| 教程领域   | 跨领域                                                           |
| 示例复杂度  | 简单                                                                     |
| 使用的 SDK            | Amazon BedrockAgentCore Python SDK 和 boto3                             |

### 教程架构

在本教程中，我们将描述如何将现有代理部署到 AgentCore runtime。

出于演示目的，我们将使用带有 Amazon Bedrock 模型的 Strands Agent。

在我们的示例中，我们将使用一个非常简单的代理，它有两个工具：`get_weather` 和 `get_time`。

<div style="text-align:left">
    <img src="images/architecture_runtime.png" width="100%"/>
</div>

### 教程主要特点

* 在 Amazon Bedrock AgentCore Runtime 上托管代理
* 使用 OpenAI 模型
* 使用 Strands Agents