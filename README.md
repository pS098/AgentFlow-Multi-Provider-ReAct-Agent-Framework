# AgentFlow-Multi-Provider-ReAct-Agent-Framework
AgentFlow is a professional-grade LLM Agent POC featuring a robust ReAct (Reasoning + Acting) loop. It orchestrates OpenAI, Anthropic, and Gemini models to execute real-time tools: Google Search, JS execution, and AI workflows. Includes a glassmorphic UI, model-agnostic architecture, and a "Zero-API" demo mode for instant testing. 🚀
# 🧠 AgentFlow

**AgentFlow** is a high-performance, model-agnostic LLM Agent Framework designed to bridge the gap between generative AI and functional task execution. It implements a **ReAct (Reasoning + Acting) loop**, allowing AI models to interact with real-world tools like web search and code execution.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-purple.svg)

## ✨ Features

* **🔄 Unified ReAct Loop:** Orchestrates complex multi-step reasoning processes across different LLM providers.
* **🤖 Multi-Model Support:** Native integration for **OpenAI** (GPT-4), **Anthropic** (Claude 3), and **Google** (Gemini 1.5).
* **🛠️ Extensible Toolbelt:** * `Google Search`: Real-time information retrieval.
    * `execute_javascript`: Safe browser-side code execution.
    * `ai_pipe`: Advanced data processing and analysis workflows.
* **🎨 Glassmorphic UI:** A professional, responsive dashboard with a modern gradient aesthetic, dark mode support, and real-time "thinking" indicators.
* **🧪 Zero-Config Demo:** Built-in mock mode to test agent workflows (like the "IBM Blog Post" scenario) without an API key.

## 🚀 Getting Started

### Prerequisites
* A modern web browser.
* (Optional) API Keys for OpenAI, Anthropic, or Google Gemini.

### Installation
1.  Clone the repository:
    ```bash
    git clone [https://github.com/yourusername/agentflow.git](https://github.com/yourusername/agentflow.git)
    ```
2.  Open `index.html` in your browser.
3.  (Optional) Enter your API keys in the settings panel to unlock live tool execution.

## 🛠️ Architecture

AgentFlow uses a **stateless-loop architecture**:
1.  **User Input:** Captured via the professional UI.
2.  **Prompt Orchestration:** The message history is formatted specifically for the selected provider (OpenAI/Anthropic/Google).
3.  **Tool Selection:** The LLM returns a structured tool call.
4.  **Local Execution:** The browser executes the tool and returns the "Observation" to the LLM.
5.  **Final Response:** Once the goal is met, the agent provides a formatted answer to the user.

## 🎨 UI Customization
The interface is built with modular CSS featuring:
- **Glassmorphism** for modern card components.
- **Dynamic Gradients** to distinguish between User, Agent, and Tool roles.
- **Mobile-Responsive**
