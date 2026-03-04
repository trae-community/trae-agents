# TRAE Agents

![TRAE Agents Banner](./assets/image/Agents.gif)

[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

[English](./README.md) | [中文](./README.zh-CN.md)

**TRAE Agents** is a community-maintained collection of custom agent configurations for the **TRAE** editor.

Here, developers share high-quality agent configuration schemes they've created, including agent names, prompts, tool configurations, and more. You can directly reference these configurations to quickly create your own agents in TRAE.

> **💡 Note**: This project focuses on **custom agent configuration schemes**. If you're looking for **MCP Servers (Tools)**, please check out [TRAE MCPs](../trae-mcp).

---

## 📖 What is a Custom Agent?

A **Custom Agent** in TRAE is an AI assistant that you configure by setting specific prompts and tools, allowing the AI to specialize in tasks within a particular domain.

Imagine creating agents like these:
- **👨‍💻 Code Review Expert**: Reviews your code and identifies potential issues
- **📝 Documentation Assistant**: Helps you write technical documentation and comments
- **🐛 Debug Expert**: Systematically helps you locate and fix bugs
- **🔧 Git Assistant**: Generates standardized commit messages and manages branches

Each agent includes the following configurations:
- **📋 Name**: The agent's identifier
- **💬 Prompt**: Defines the agent's role, objectives, and workflow
- **🛠️ Tools**: Callable MCP services and other capabilities
- **🤝 Collaboration**: Other agents that can be invoked

## 🚀 Features

- **Ready to Use**: Provides validated agent configuration schemes
- **Community Driven**: Gathers wisdom from developers worldwide
- **Fully Transparent**: Publishes all configuration details, including prompts and tool settings
- **Easy to Reuse**: Clear import guide for quick creation in TRAE

## 📦 Agent List

| Agent Name | Description | Status | Documentation |
| :--- | :--- | :--- | :--- |
| git-commit-generator | Generate Git commit messages following Conventional Commits specification | ✅ Stable | [Configuration Details](./agents/git-commit-generator/) |
| (To be added) | More agents under development... | 🚧 | - |

*(The repository is currently initializing. PRs to contribute your agent configurations are welcome!)*

## 🛠️ How to Use

### Step 1: Browse Agents
Browse the agent list above to find the agent you need.

### Step 2: View Configuration Details
Click on the agent name to view complete configuration information, including:
- Agent name
- Full prompt text
- Tool configuration
- Usage examples

### Step 3: Create in TRAE

#### 3.1 Open TRAE
Launch the TRAE editor.

#### 3.2 Access Agent Management
- Click the agent icon (🤖) in the left sidebar
- Select "Manage Agents" or "Create New Agent"

#### 3.3 Fill in Configuration

**Name**:
Enter the agent name, e.g., `Git Commit Generator`

**Prompt**:
Copy the provided complete prompt content and paste it into the Prompt input box.

**Tools**:
Check the recommended built-in tools based on recommendations:
- File editing
- Terminal commands
- Web search
- Browser automation

**MCP Servers (Optional)**:
If the agent requires MCP services, add them according to the provided JSON configuration.

**Other Agents (Optional)**:
If you need to invoke other agents, add their names.

#### 3.4 Save and Test
- Click "Save" to save
- Return to the chat interface
- Try testing the agent with inputs from the examples

### Step 4: Adjust and Optimize
Based on actual usage experience, you can:
- Adjust the wording of prompts
- Add or remove tools
- Modify constraints
- Optimize workflows

## 🤝 How to Contribute

We welcome and appreciate community contributions! If you've configured a useful agent, please follow these steps to share:

1. Read the [Contribution Guidelines](./CONTRIBUTING.md)
2. Fork this repository and create a new branch
3. Create your agent configuration directory under the `agents/` directory
4. Provide complete configuration information following the template format
5. Update the **Agent List** section
6. Submit a Pull Request

## 📚 Agent Development Resources

- [TRAE Agent Overview](https://docs.trae.ai/ide/agent-overview)
- [Create and Manage Agents](https://docs.trae.ai/ide/agent)
- [Best Practices for Agent Skills](https://www.trae.ai/blog/trae_tutorial_0115?v=1)

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=trae-community/trae-agents&type=Date)](https://www.star-history.com/#trae-community/trae-agents&Date)

## Disclaimer

The agent configurations in this repository are provided for community exchange and learning purposes only. Please fully test and adjust them before using them in production or security-sensitive scenarios.

## Links

- TRAE Official Website: https://www.trae.ai/
- TRAE Documentation: https://docs.trae.ai/
