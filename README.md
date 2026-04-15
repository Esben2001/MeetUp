🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎲 Soc Ops

> **Break the ice at networking events.** Social Bingo transforms awkward mixers into fun conversations. Find people matching questions on your card and get 5 in a row to win!

[![Play the Game](https://img.shields.io/badge/🎮_Play_Now-5A67D8?style=for-the-badge&labelColor=2D3748)](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)
[![View Lab Guide](https://img.shields.io/badge/📚_Learning_Path-38A169?style=for-the-badge&labelColor=2D3748)](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/)

---

## ✨ What Makes Soc Ops Great?

🎯 **Icebreaker Superpower** — Naturally start conversations with meaningful questions  
👥 **Interactive Gameplay** — Tap squares as you find people with matching stories  
🏆 **Quick Wins** — Get 5 in a row to celebrate and build momentum  
🎨 **Smooth Design** — Built with modern Blazor for a responsive experience  
⚡ **Instant Setup** — Run it locally or jump straight into the [live demo](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)  

---

## 🚀 Quick Start

### Prerequisites
- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or higher

### Run Locally

```bash
cd SocOps
dotnet run
```

Open your browser and start networking! 🎉

### Open in GitHub Codespaces (Optional)

1. Click **Code** → **Codespaces** → **Create codespace on main**
2. Wait for the devcontainer to finish
3. From the repository root:
   ```bash
   cd SocOps
   dotnet run
   ```

---

## 📚 Learning Path

Master .NET development with a hands-on lab experience building Soc Ops:

| Part | Topic | Learn |
|------|-------|-------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Overview & Checklist | Project setup & goals |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Setup & Context Engineering | Configure your dev environment |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Design-First Frontend | Build polished Blazor components |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Custom Quiz Master | Create dynamic content systems |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Multi-Agent Development | Orchestrate AI-powered workflows |

> 📖 Prefer offline? Lab guides are available in the [`workshop/`](workshop/) folder.
---

## 🛠️ Build & Deploy

### Build

```bash
cd SocOps
dotnet build
```

### Deploy

Pushes to `main` automatically deploy to GitHub Pages. No additional setup needed!

---

## 🎯 Game Mechanics

**How to Play:**
1. **Start** the game to get your bingo card
2. **Find people** at the event who match the questions on your squares
3. **Tap squares** as you connect with others
4. **Get 5 in a row** (horizontal, vertical, or diagonal) to win!

**Sample Questions:**
- 🚴 Bikes to work
- 🌍 Has lived in another country
- 🐾 Has a pet
- ☕ Prefers tea over coffee
- 🎸 Plays an instrument
- 🗣️ Speaks more than 2 languages
- 🪂 Has been skydiving
- 🎬 Has been on TV

---

## 📦 Tech Stack

Built with modern, production-ready technologies:

- **Frontend:** [Blazor WebAssembly](https://dotnet.microsoft.com/en-us/apps/aspnet/web-apps/blazor) for interactive web UIs
- **Backend:** C# with .NET 10
- **Storage:** Browser localStorage for game state
- **Styling:** Custom CSS utilities for a distinctive design

---

## 📖 Project Structure

```
SocOps/
├── Components/      # Blazor UI components (Board, Modal, Squares)
├── Services/        # Game logic & state management
├── Models/          # Core data types (GameState, BingoLine)
├── Data/            # Question bank & static data
├── Pages/           # Application pages
└── wwwroot/         # Static assets & stylesheets
```

---

## 🤝 Contributing

We welcome contributions! Check out [CONTRIBUTING.md](CONTRIBUTING.md) to get started.

**Report Issues:** [GitHub Issues](../../issues)  
**Security:** See [SECURITY.md](SECURITY.md) for reporting security vulnerabilities  
**Code of Conduct:** We're committed to a welcoming community — read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

---

## 📜 License

Soc Ops is licensed under the [MIT License](LICENSE).

---

## 💡 Questions or Feedback?

Have ideas to improve the game or found a bug? [Open an issue](../../issues/new) — we'd love to hear from you!

**Join the Community:**
- 🎮 [Play the live demo](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)
- 📚 [Read the full lab guide](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/)
- 💬 [Start a discussion](../../discussions)
