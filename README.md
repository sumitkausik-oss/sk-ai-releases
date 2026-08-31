# SK-AI — Advanced AI Desktop Assistant

**SK-AI** is a desktop AI system built by **Sumeet Kumar**. It integrates advanced LLM reasoning, voice synthesis, autonomous browser automation, Python runtime execution, desktop accessibility assistance, and local multi-agent collaboration.

---

## 🌟 Key Features

* **Universal Assistant**: Multi-modal chat, code generation, file analysis, system automation, and intelligent Butler persona.
* **Autonomous Browser Control**: Built-in Chromium automation via Chrome DevTools Protocol (CDP) for web scraping, navigation, and automated interactions.
* **Hermes Multi-Agent Runtime**: Embedded Python runtime environment enabling local tool calling, web search, code interpretation, and persistent memory.
* **Voice & Wake-Word Detection**: Always-on background wake-word engine ("SK-AI", "Sky AI") with voice feedback.
* **Freeware Edition**: 100% unlocked offline architecture with no remote licensing or token server dependencies.
* **AgentTown Workspace**: Embedded multi-agent simulation canvas and interactive companion interfaces.

---

## 🚀 Architecture & Local Services

| Service | Technology | Port / Endpoint | Description |
| :--- | :--- | :--- | :--- |
| **Desktop Shell** | Electron / Node.js | Local IPC | Main window management, IPC handlers, system integrations |
| **Frontend UI** | React 19 / Vite / Tailwind | Local Window / PWA | Main user dashboard, chat, settings, and widget controls |
| **AgentTown Server**| Next.js Standalone Bundle | `http://127.0.0.1:3010` | Embedded agent town simulation and API routes |
| **Hermes Runtime** | Python 3.11 Embedded | `http://127.0.0.1:9119` | Local tool-calling, skills execution, and memory storage |
| **CDP Shim** | Node.js HTTP/WS | `http://127.0.0.1:9222` | Browser automation bridge for Chromium |
| **Voice Engine** | Python SpeechRecognition | Background Child Process| Background wake-word listener |

---

## 📂 Installation & Running

### Option 1: Standalone Portable Release
1. Extract `release/application/` to any folder (e.g. `C:\Program Files\SK-AI` or `C:\Users\<User>\AppData\Local\Programs\SK-AI`).
2. Run `SK AI.exe` (or `SK-AI.exe`).

### Option 2: Windows Installer
1. Run `SK-AI-Setup-1.0.52.exe`.
2. Follow standard setup instructions. The application will install to your local app directory and create desktop and start menu shortcuts.

---

## ⚙️ Configuration & Environment

Environment variables can be set to override local subservice ports:

* `SK_AI_AGENTTOWN_PORT`: Port for AgentTown server (Default: `3010`)
* `SK_AI_HERMES_PORT`: Port for Hermes runtime engine (Default: `9119`)
* `SK_AI_CDP_SHIM_PORT`: Port for Chromium DevTools Protocol shim (Default: `9222`)
* `SK_AI_HERMES_EXE`: Custom executable path for Hermes Python runtime

---

## 👤 Author & Credits

* **Product**: SK-AI
* **Creator / Architect**: Sumeet Kumar
* **Edition**: Standalone Freeware
* **License**: Freeware (Free for all users by Sumeet Kumar)
* **Copyright**: &copy; 2026 Sumeet Kumar. All rights reserved.
