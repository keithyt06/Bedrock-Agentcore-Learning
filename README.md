# Amazon Bedrock AgentCore 示例

欢迎来到 Amazon Bedrock AgentCore 示例仓库！

> [!CAUTION]
> 本仓库中提供的示例仅用于实验和教育目的。它们展示了概念和技术，但不适合直接在生产环境中使用。请确保使用 Amazon Bedrock Guardrails 来防止[提示注入](https://docs.aws.amazon.com/bedrock/latest/userguide/prompt-injection.html)。

**Amazon Bedrock AgentCore** 是一套完整的功能集，可使用任何代理框架和任何 LLM 模型安全地大规模部署和运行代理。
借助它，开发人员可以快速将 AI 代理投入生产，加速业务价值实现。

Amazon Bedrock AgentCore 提供工具和功能，使代理更加高效和强大，提供专为安全扩展代理而构建的基础设施，以及
控制可信代理运行的机制。

Amazon Bedrock AgentCore 功能可组合使用，并与流行的开源框架和任何模型配合使用，因此您无需在
开源灵活性和企业级安全性及可靠性之间做出选择。

此集合提供示例和教程，帮助您了解、实现和将 Amazon Bedrock AgentCore 功能集成到您的应用程序中。

## 📁 仓库结构

### 📚 [`01-tutorials/`](./01-tutorials/)
**交互式学习与基础**

此文件夹包含基于笔记本的教程，通过实践示例教您 Amazon Bedrock AgentCore 功能的基础知识。

结构按 AgentCore 组件划分：
* **Runtime**：Amazon Bedrock AgentCore Runtime 是一种安全、无服务器的运行时功能，使组织能够部署和扩展 AI 代理和工具，无论框架、协议或模型选择如何——实现快速原型设计、无缝扩展和加速上市时间
* **Gateway**：AI 代理需要工具来执行现实世界的任务——从搜索数据库到发送消息。Amazon Bedrock AgentCore Gateway 自动将 API、Lambda 函数和现有服务转换为 MCP 兼容工具，使开发人员无需管理集成即可快速使这些基本功能可供代理使用。
* **Memory**：Amazon Bedrock AgentCore Memory 使开发人员能够轻松构建丰富、个性化的代理体验，具有完全管理的内存基础设施和根据需求自定义内存的能力。
* **Identity**：Amazon Bedrock AgentCore Identity 提供跨 AWS 服务和第三方应用程序（如 Slack 和 Zoom）的无缝代理身份和访问管理，同时支持任何标准身份提供商，如 Okta、Entra 和 Amazon Cognito。
* **Tools**：Amazon Bedrock AgentCore 提供两个内置工具来简化您的代理式 AI 应用程序开发：Amazon Bedrock AgentCore **Code Interpreter** 工具使 AI 代理能够安全地编写和执行代码，提高其准确性并扩展其解决复杂端到端任务的能力。Amazon Bedrock AgentCore **Browser Tool** 是一种企业级功能，使 AI 代理能够导航网站、完成多步骤表单，并在完全管理、安全的沙盒环境中以低延迟执行复杂的基于网络的任务，具有类人精度
* **Observability**：Amazon Bedrock AgentCore Observability 通过统一的操作仪表板帮助开发人员跟踪、调试和监控代理性能。通过支持与 OpenTelemetry 兼容的遥测和代理工作流每个步骤的详细可视化，Amazon Bedrock AgentCore Observability 使开发人员能够轻松获得代理行为的可见性并大规模维护质量标准。

**端到端示例**文件夹提供了如何在用例中组合不同功能的简单示例。

提供的示例非常适合初学者和那些希望在构建 AI 代理应用程序之前了解基本概念的人。

### 💡 [`02-use-cases/`](./02-use-cases/)
**端到端应用**

探索实际用例实现，展示如何应用 Amazon Bedrock AgentCore 功能解决实际业务问题。

每个用例都包括完整的实现，重点关注 AgentCore 组件，并提供详细说明。

### 🔌 [`03-integrations/`](./03-integrations/)
**框架与协议集成**

了解如何将 Amazon Bedrock AgentCore 功能与流行的代理框架（如 Strands Agents、LangChain 和 CrewAI）集成。

设置代理到代理的通信（A2A）和不同的多代理协作模式。集成代理接口，并了解如何使用
不同入口点的 Amazon Bedrock AgentCore。

## 🚀 快速开始

1. **克隆仓库**

   ```bash
   git clone https://github.com/awslabs/amazon-bedrock-agentcore-samples.git
   ```

2. **设置环境**

   ```bash
   pip install bedrock-agentcore
   ```

3. **从教程开始**
   ```bash
   cd 01-tutorials
   jupyter notebook
   ```

## 📋 先决条件

- Python 3.10 或更高版本
- AWS 账户
- Jupyter Notebook（用于教程）

## 🤝 贡献

我们欢迎贡献！请查看我们的[贡献指南](CONTRIBUTING.md)了解以下详情：

- 添加新样例
- 改进现有示例
- 报告问题
- 提出改进建议

## 📄 许可证

本项目采用 MIT 许可证 - 详情请参阅[LICENSE](LICENSE)文件。

## 🆘 支持

- **问题**：通过[GitHub Issues](https://github.com/awslabs/amazon-bedrock-agentcore-samples/issues)报告错误或请求功能
- **文档**：查看各个文件夹的 README 获取具体指导

## 🔄 更新

本仓库正在积极维护和更新，添加新功能和示例。关注仓库以获取最新添加内容的更新。