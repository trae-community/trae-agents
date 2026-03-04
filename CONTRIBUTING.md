# Contribution Guidelines

Welcome to submit PRs! We recommend keeping each agent "small and specialized" and focused on solving problems in specific scenarios.

![TRAE Agents Banner](./assets/image/Agents.gif)

[English](./CONTRIBUTING.md) | [中文](./CONTRIBUTING.zh-CN.md)

## 🚀 Create a New Agent

### 1. Fork the Repository and Create a Branch
```bash
git checkout -b feature/your-agent-name
```

### 2. Create Agent Directory
- Create a new folder in the `agents/` directory
- Use kebab-case naming: `your-agent-name`
- Copy the template file `agents/_template/README.md` to your directory

### 3. Fill in Configuration Information
Fill in the following content according to the template requirements:

#### ✅ Required Sections
- **Basic Information**: Name, description, applicable scenarios
- **Prompt**: Complete system instructions
- **Usage Examples**: At least 1 input-output example

#### 🔧 Optional Sections
- **MCP Service Configuration**: If MCP is needed
- **Tool Configuration**: Recommended built-in tools
- **Collaborative Agents**: Other agents that can work together
- **Configuration Suggestions**: Model selection, parameter settings, etc.
- **Related Resources**: Documentation and reference links

### 4. Test Your Agent
Actually create and test in TRAE:
1. Open TRAE
2. Create an agent according to your written configuration
3. Test with different inputs
4. Optimize prompts based on test results

### 5. Update README
Add your agent to the agent list in `README.md`:
```markdown
| your-agent-name | One-line description | ✅ Stable | [Configuration Details](./agents/your-agent-name/) |
```

### 6. Submit PR
- Ensure all files are committed
- Write clear commit messages
- Push to your fork
- Create Pull Request

## 📋 Quality Standards

Your agent should meet the following requirements:

### ✅ Content Requirements
- **Clear Positioning**: Clearly explain what this agent does
- **Complete Prompt**: Include role definition, objectives, workflow, and constraints
- **Practical Examples**: Show real input-output examples
- **Reproducible**: Others can create agents with the same effect following your configuration

### ❌ Issues to Avoid
- Do not include sensitive information (API keys, tokens, internal URLs, etc.)
- Do not be too broad (one agent doing everything)
- Do not lack examples
- Do not use vague instructions (like "do your best")

## 📁 File Structure

Each agent directory should include:

```
your-agent-name/
├── README.md          # Main configuration file (required)
└── resources/        # Related resource files (optional)
    └── reference.md
```

## 🏷️ Status Indicators

Use emoji indicators for agent status in README:

- 🚧 **Under Development**: Still testing, may be adjusted
- ✅ **Stable**: Tested and working well
- ⚠️ **Deprecated**: Still available but not recommended for new use

## 🎯 Naming Conventions

### Agent Name
- Use English with capitalized first letters: `Git Commit Generator`
- Or use kebab-case: `git-commit-generator`
- Clearly express the purpose, avoid ambiguity

### Directory Name
- Must use kebab-case: `git-commit-generator`
- All lowercase
- Clear and concise

## ✅ PR Checklist

Before submitting, please confirm:

- [ ] Created agent directory and README.md
- [ ] Includes complete Prompt (can be directly copied to TRAE)
- [ ] Provided at least 1 usage example
- [ ] No sensitive information (API keys, tokens, etc.)
- [ ] Updated the main README agent list
- [ ] Actually tested in TRAE
- [ ] Followed the template structure
- [ ] Used correct naming conventions

## 💡 Best Practices

### Tips for Writing Good Prompts

1. **Clear Role**: "You are an XXX expert"
2. **Define Objectives**: "Your responsibility is to..."
3. **Step by Step**: "First step... Second step..."
4. **Give Examples**: "For example..."
5. **State Constraints**: "Do not..."

### Common Patterns

#### Analysis + Recommendation Type
```
You are a code review expert. When users provide code:
1. Analyze code structure and logic
2. Identify potential issues
3. Provide improvement suggestions
```

#### Task Execution Type
```
You are a Git assistant. When users need to write commit messages:
1. Read code changes
2. Determine change type
3. Generate standardized commit messages
```

#### Q&A Consulting Type
```
You are a technical consultant. When answering user technical questions:
1. Understand the core of the problem
2. Provide multiple solutions
3. Analyze pros and cons of each solution
```

## 🤔 Frequently Asked Questions

### Q: How long should the Prompt be?
A: There's no fixed standard, typically 200-500 words is appropriate. The key is to be clear and complete, not longer is better.

### Q: Do I need to configure MCP?
A: Most agents don't need it. Only use when you really need to access external data or services.

### Q: How to test the effect?
A: After creating in TRAE, test with 3-5 different real scenarios to see if they all give reasonable responses.

### Q: Can I reference other agents?
A: Yes, but ensure the referenced agents already exist and are stable.

## 📚 Reference Resources

- [TRAE Official Documentation](https://docs.trae.ai/ide/agent)
- [Best Practices for Agent Skills](https://www.trae.ai/blog/trae_tutorial_0115?v=1)
- [Prompt Engineering Guide](https://github.com/datawhalechina/prompt-engineering-for-developers)

## 🙏 Acknowledgments

Thank you to every developer contributing wisdom to the community! 🎉

Feel free to discuss any questions through Issues.
