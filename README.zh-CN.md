# TRAE Agents

![TRAE Agents Banner](./assets/image/Agents.gif)

[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

[English](./README.md) | [中文](./README.zh-CN.md)

**TRAE Agents** 是一个社区维护的 TRAE 自定义智能体配置集合。

在这里，开发者分享自己创建的高质量智能体配置方案，包括智能体名称、提示词（Prompt）、工具配置等。你可以直接参考这些配置，在 TRAE 中快速创建属于自己的智能体。

> **💡 提示**：本项目专注于**自定义智能体配置方案**。如果你在寻找 **MCP Servers (工具)**，请查看 [TRAE MCPs](../trae-mcp)。

---

## 📖 什么是自定义智能体？

TRAE 中的**自定义智能体**是你自己配置的 AI 助手，通过设置特定的提示词和工具，让 AI 专门擅长某个领域的任务。

想象一下，你可以创建这样的智能体：
- **👨‍💻 代码审查专家**：专门帮你 review 代码，发现潜在问题
- **📝 文档写作助手**：帮助你编写技术文档和注释
- **🐛 Debug 专家**：系统性地帮你定位和解决 bug
- **🔧 Git 助手**：生成规范的 commit message、管理分支

每个智能体包含以下配置：
- **📋 名称**：智能体的标识
- **💬 提示词（Prompt）**：定义智能体的角色、目标和工作流程
- **🛠️ 工具**：可调用的 MCP 服务和其他能力
- **🤝 协作**：可调用的其他智能体

## 🚀 特性

- **即取即用**：提供经过验证的智能体配置方案
- **社区驱动**：汇聚全球开发者的智慧和最佳实践
- **完全透明**：公开所有配置细节，包括提示词和工具设置
- **易于复用**：清晰的导入指南，快速在 TRAE 中创建

## 📦 智能体列表

| Agent Name | Description | Status | Documentation |
| :--- | :--- | :--- | :--- |
| git-commit-generator | 生成符合 Conventional Commits 规范的 Git 提交信息 | ✅ Stable | [配置详情](./agents/git-commit-generator/) |
| (待添加) | 更多智能体正在开发中... | 🚧 | - |

*(仓库目前正在初始化中，欢迎提交 PR 贡献你的智能体配置！)*

## 🛠️ 如何使用

### 步骤 1：选择智能体
浏览上面的智能体列表，找到你需要的智能体。

### 步骤 2：查看配置详情
点击智能体名称，查看完整的配置信息，包括：
- 智能体名称
- 提示词（Prompt）全文
- 工具配置
- 使用示例

### 步骤 3：在 TRAE 中创建

#### 3.1 打开 TRAE
启动 TRAE 编辑器。

#### 3.2 进入智能体管理
- 点击左侧边栏的智能体图标（🤖）
- 选择 "Manage Agents" 或 "创建新智能体"

#### 3.3 填写配置

**Name（名称）**:
输入智能体名称，例如 `Git Commit Generator`

**Prompt（提示词）**:
复制提供的完整提示词内容，粘贴到 Prompt 输入框。

**Tools（工具）**:
根据推荐勾选内置工具：
- 文件编辑
- 终端命令
- 网络搜索
- 浏览器自动化

**MCP Servers（可选）**:
如果智能体需要 MCP 服务，按照提供的 JSON 配置添加。

**Other Agents（可选）**:
如果需要调用其他智能体，添加它们的名称。

#### 3.4 保存并测试
- 点击 "Save" 保存
- 回到聊天界面
- 尝试用示例中的输入测试智能体

### 步骤 4：调整优化
根据实际使用体验，你可以：
- 调整提示词的措辞
- 添加或删除工具
- 修改约束条件
- 优化工作流程

## 🤝 如何贡献

我们欢迎并感谢社区的贡献！如果你配置了一个好用的智能体，请按照以下步骤分享：

1. 阅读 [贡献指南](./CONTRIBUTING.md)
2. Fork 本仓库并创建新分支
3. 在 `agents/` 目录下创建你的智能体配置目录
4. 按照模板格式提供完整配置信息
5. 更新 **智能体列表** 部分
6. 提交 Pull Request

## 📚 智能体开发资源

- [TRAE 智能体概述](https://docs.trae.ai/ide/agent-overview?_lang=zh)
- [创建和管理智能体](https://docs.trae.ai/ide/agent?_lang=zh)
- [智能体技能最佳实践](https://www.trae.ai/blog/trae_tutorial_0115?v=1)

## 📄 许可证

本项目采用 [MIT 许可证](LICENSE)。

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=trae-community/trae-agents&type=Date)](https://www.star-history.com/#trae-community/trae-agents&Date)

## 免责声明

本仓库中的智能体配置仅供社区交流和学习使用。请在用于生产或安全敏感场景之前进行充分测试和调整。

## 链接

- TRAE 官网：https://www.trae.ai/
- TRAE 文档：https://docs.trae.ai/
