# code-assistant


<div align="center">

![Code Assistant](https://img.shields.io/badge/Code-Assistant-blue)
![Python](https://img.shields.io/badge/Python-3.11+-green)
![License](https://img.shields.io/badge/License-LGPL%203.0-lightgrey)
![Version](https://img.shields.io/badge/Version-0.2.4-orange)

**An AI-powered coding assistant with DeepSeek integration and advanced function calling capabilities**

[Documentation](https://selobu.github.io/code-assistant/) • [Installation](#installation) • [Quick Start](#quick-start) • [Features](#features)

</div>

## 🚀 Overview

Code Assistant is a sophisticated AI-powered development tool that helps developers write better code, faster. With DeepSeek's advanced reasoning models and comprehensive function calling capabilities, it provides expert-level code analysis, file operations, git integration, and project context management.

### ✨ Key Features

- **🤖 AI-Powered Code Analysis** - Expert-level insights and explanations
- **🔧 Function Calling Tools** - Direct file and system operations
- **📁 Project Context** - Maintain memory across conversations
- **👤 Custom Profiles** - Specialized AI behavior for different domains
- **🔐 Secure Authentication** - Multiple API key management methods
- **🧠 Memory Management** - Persistent context across sessions

## 🛠️ Installation

### Quick Install

```bash
# Basic installation
pip install code-assistant

# With development dependencies
pip install "code-assistant[dev]"

# With documentation dependencies
pip install "code-assistant[docs]"
```

### From Source

```bash
git clone https://github.com/selobu/code-assistant.git
cd code-assistant
pip install -e ".[dev,docs]"
```

### Prerequisites

- Python 3.11 or higher
- DeepSeek API key ([Get one here](https://platform.deepseek.com))

## 🚀 Quick Start

### 1. Set API Key

```bash
# Interactive setup
code-assistant --auth

# Or set directly
code-assistant --auth-key sk-your-api-key-here

# Or use environment variable
export DEEPSEEK_API_KEY="sk-your-api-key-here"
```

### 2. Start Coding

```bash
# Start interactive session
code-assistant

# Example usage
You> Explain what this code does and suggest improvements
You> Create a user authentication module
You> Add tests for the new feature
```

## 📚 Documentation

Comprehensive documentation is available at: **[https://selobu.github.io/code-assistant/](https://selobu.github.io/code-assistant/)**

### Key Documentation Sections

- **[Getting Started](docs/getting-started.md)** - Installation and basic usage
- **[Configuration Guide](docs/configuration.md)** - Customization and settings
- **[Profile Management](docs/profiles.md)** - Custom AI behavior profiles
- **[Tools Reference](docs/tools/index.md)** - Function calling capabilities
- **[Memory Tool Guide](docs/tools/memory-tool.md)** - Cross-conversation context
- **[Development Guide](docs/development.md)** - Contributing to the project

## 🎯 Features

### AI-Powered Assistance
- Natural language conversations about code
- Expert-level insights across all programming domains
- Code optimization and best practices
- Architecture review and system design

### Function Calling Tools
- **File Operations**: Read, create, edit, move files
- **Git Integration**: Analyze changes, suggest commits
- **Project Analysis**: Directory scanning, context management
- **Environment Management**: Python environment setup
- **Memory Management**: Persistent context across conversations

### Project Context Management
- Maintain project memory across conversations
- Store and retrieve project analysis data
- Understand large codebases quickly
- Preserve context across multiple interactions

### Custom Profile System
- Create specialized AI behavior profiles
- Team collaboration with shared profiles
- Project-specific expertise requirements
- Export/import profile configurations

### Advanced Prompt System
- Domain-specific prompts for specialized expertise
- Simplified prompts for token optimization
- Custom prompt creation for specific needs
- Cost-effective interactions through prompt optimization

## 🔧 Usage Examples

### Code Analysis

```bash
# Analyze existing code
You> What improvements can we make to src/main.py code?
You> How can we optimize performance?
```

### File Operations

```bash
# Create new files
You> Create a REST API with CRUD operations for a User model

# Edit existing code
You> Add error handling to the database connection

# Reorganize project structure
You> Move utils.py to src/utils/
```

### Project Context

```bash
# Save project context for later
You> /context save

# Load context in new session
You> /context load

# Get project overview
You> /structure
```

### Custom Profiles

```bash
# Create specialized profile
/profile create "Python Expert" python_expert "You are a Python programming expert..."

# Use the profile
/profile use python_expert
```

## 🏗️ Architecture

### Core Components

- **Assistant Core** - AI conversation management and tool coordination
- **Tool System** - Modular function calling with file operations, git integration, etc.
- **Memory Management** - Persistent context storage and retrieval
- **Profile System** - Customizable AI behavior and expertise
- **Configuration System** - Layered settings management

### Tool Integration

The assistant integrates with:
- **File System** - Direct file operations with precision editing
- **Git** - Version control with intelligent commit analysis
- **Python Environment** - Dependency management and testing
- **Project Analysis** - Directory structure and code understanding

## 🧪 Testing

```bash
# Run all tests
pytest

# Run with coverage
pytest --cov=code_assistant

# Run specific test categories
pytest tests/unit/
pytest tests/integration/
```

## 🤝 Contributing

We welcome contributions! Please see our [Development Guide](docs/development.md) for details.

### Development Setup

```bash
# Clone and setup
git clone https://github.com/selobu/code-assistant.git
cd code-assistant
pip install -e ".[dev,docs]"

# Run tests
pytest

# Format code
black .
flake8 .
```

### Contribution Areas

- New function calling tools
- Enhanced memory management
- Additional domain prompts
- Performance optimizations
- Documentation improvements
- Bug fixes and testing

## 📊 Project Status

- **Version**: 0.2.4
- **Status**: Active development
- **Python Support**: 3.11+
- **License**: LGPL 3.0

## 🔒 Security

- API keys stored securely using system keyring
- Encrypted fallback storage
- No sensitive data logged
- Input validation and sanitization

## 📄 License

This project is licensed under the LGPL 3.0 License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built on [DeepSeek](https://www.deepseek.com/) AI models
- Inspired by modern AI-assisted development tools
- Community contributions and feedback

## 📞 Support

- **Documentation**: [https://selobu.github.io/code-assistant/](https://selobu.github.io/code-assistant/)
- **Issues**: [GitHub Issues](https://github.com/selobu/code-assistant/issues)
- **Discussions**: [GitHub Discussions](https://github.com/selobu/code-assistant/discussions)

---

<div align="center">

**Happy coding! 🚀**

*Code Assistant - Your AI-powered development companion*
*Making developers more productive, one conversation at a time*

[⭐ Star us on GitHub](https://github.com/selobu/code-assistant) • [📚 Read the Docs](https://selobu.github.io/code-assistant/) • [🐛 Report Issues](https://github.com/selobu/code-assistant/issues)

</div>

Latest version 0.2.6
