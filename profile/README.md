# Altair

> ADHD-friendly productivity ecosystem that works offline-first

[![License](https://img.shields.io/badge/license-AGPL--3.0-blue.svg)](https://github.com/getaltair/altair/blob/main/LICENSE)
[![Flutter](https://img.shields.io/badge/Flutter-3.0+-02569B?logo=flutter)](https://flutter.dev)
[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?logo=python)](https://python.org)
[![Status](https://img.shields.io/badge/status-Phase%201%20Complete-brightgreen)]()

---

## 🎯 What We're Building

**Three focused apps for ADHD project management:**

1. **🎯 Guidance** - Task & project management (Beta Ready - Week 12)
2. **📚 Knowledge** - Personal wiki & notes (Phase 2 - Planned)
3. **📦 Tracking** - Inventory & resources (Phase 3 - Planned)

**Why ADHD-friendly?**
- ⚡ **Quick capture** - Thought to save in under 3 seconds
- 🏠 **Works offline** - No internet required, sync is optional
- 🎨 **Visual clarity** - High contrast, clear feedback
- 🤖 **AI-powered** - Break down tasks automatically
- 🔐 **Private first** - Your data stays on your device

---

## ⚡ Quick Start

**Try Altair Guidance (Task Management):**

```bash
# Clone and run
git clone https://github.com/getaltair/altair.git
cd altair/apps/altair-guidance
flutter pub get
flutter run -d linux  # or macos, windows
```

**You should see:** The Altair Guidance app launch with a quick capture screen

---

## 🚀 Key Features

### Works Without Internet
- All apps run **100% offline** by default
- Enable sync later when you need multi-device access
- Your data stays on your device

### Built for ADHD
- **Quick capture** - No friction between thought and action
- **Visual time tracking** - Combat time blindness
- **AI task breakdown** - Prevent overwhelm
- **Neo-brutalist UI** - Clear visual hierarchy

### Local-First Architecture
- **Download and run** - No setup required
- **Optional sync** - Add when you need it
- **Fast** - Instant saves, sub-second page loads
- **Private** - You control your data

---

## 📱 The Apps

### 🎯 Altair Guidance (Phase 1: Beta Ready)
**Task and project management for ADHD**

**Implemented features:**
- ✅ Quick capture (< 3 seconds)
- ✅ Task & project management
- ✅ AI-powered features (OpenAI, Anthropic, Ollama)
- ✅ Neo-brutalist UI with ADHD-friendly design
- ✅ Offline-first with SQLite
- ✅ Standalone installers (Linux, macOS, Windows)

**Status:** 🚀 Week 12 - Beta testing with standalone installers
**Next:** Phase 2 - Altair Knowledge (Wiki/Notes)

[View Guidance README →](https://github.com/getaltair/altair/tree/main/apps/altair_guidance)

### 📚 Altair Knowledge (Phase 2: Planned)
**Personal wiki and knowledge management**

**Planned features:**
- Markdown-based notes
- Automatic backlinks & graph view
- Daily notes
- Cross-app linking with Guidance

**Status:** 📋 Phase 2 - Not yet started

### 📦 Altair Tracking (Phase 3: Planned)
**Inventory and resource management**

**Planned features:**
- Barcode scanning
- Location-based organization
- Smart alerts (low stock, expiration)
- Integrates with tasks and wiki

**Status:** 📋 Phase 3 - Not yet started

---

## 🏗️ Architecture

```
Standalone Mode (Default)        Sync Mode (Optional)
┌─────────────────┐             ┌─────────────────┐
│  Flutter App    │             │  Flutter App    │
│       +         │             │       +         │
│    SQLite       │             │ SQLite + Sync   │
└─────────────────┘             └────────┬────────┘
                                         │
                                    ┌────▼────────┐
                                    │  FastAPI    │
                                    │     +       │
                                    │ PostgreSQL  │
                                    └─────────────┘
```

**Key decisions:**
- ✅ **Local-first** - Apps work standalone
- ✅ **Progressive** - Add features when needed
- ✅ **Proven tech** - SQLite, PostgreSQL, PowerSync

[Architecture Details →](https://github.com/getaltair/altair/blob/main/docs/ARCHITECTURE-OVERVIEW.md)

---

## 🛠️ Technology Stack

**Frontend:**
- Flutter (cross-platform)
- SQLite (local database)
- Bloc (state management)

**Backend (Optional):**
- FastAPI (Python)
- PostgreSQL (server database)
- PowerSync (sync engine)

**AI Integration:**
- OpenAI (GPT-4)
- Anthropic (Claude)
- Ollama (local models)

---

## 📚 Documentation

### For Users
- [Getting Started](https://github.com/getaltair/altair#quick-start) - Run Altair Guidance
- [Development Roadmap](https://github.com/getaltair/altair/blob/main/docs/DEVELOPMENT-ROADMAP.md) - What's coming next

### For Developers
- [Architecture Overview](https://github.com/getaltair/altair/blob/main/docs/ARCHITECTURE-OVERVIEW.md) - How it all works
- [Data Flow](https://github.com/getaltair/altair/blob/main/docs/DATA-FLOW.md) - Understanding data movement
- [Component Design](https://github.com/getaltair/altair/blob/main/docs/COMPONENT-DESIGN.md) - Code structure
- [Contributing Guide](https://github.com/getaltair/altair/blob/main/CONTRIBUTING.md) - How to contribute

---

## 🎯 Current Status

**Phase 1: Altair Guidance** (Weeks 1-12) - ✅ COMPLETE

- ✅ Month 1: Infrastructure & Authentication
  - CI/CD pipeline with GitHub Actions
  - Monorepo structure
  - Backend services (FastAPI, auth-service)
  - Core packages (altair-ui, altair-core, altair-auth)

- ✅ Month 2: Core Task Management
  - Quick capture widget (< 3 sec)
  - Task & project CRUD operations
  - Task editing and filtering
  - SQLite local storage with migrations

- ✅ Month 3: AI Integration & Polish
  - OpenAI, Anthropic, and Ollama support
  - AI-powered task breakdown
  - Settings UI with provider selection
  - Comprehensive testing suite

- ✅ Week 12: Beta & Distribution
  - Standalone installers (Linux AppImage, macOS DMG, Windows Setup)
  - Beta testing in progress
  - Documentation complete

**Next:** Phase 2 - Altair Knowledge (Personal Wiki)

[View Detailed Roadmap →](https://github.com/getaltair/altair/blob/main/docs/DEVELOPMENT-ROADMAP.md)

---

## 🤝 Contributing

We welcome contributions from:
- **Developers** - Flutter, Python, or both
- **Designers** - UI/UX, especially ADHD-friendly design
- **ADHD community** - Feedback and testing
- **Documentation writers** - Help make docs accessible

### Quick Contribution Guide

1. **Find an issue** - Look for `good-first-issue` label
2. **Fork and clone** - Get the code locally
3. **Make changes** - Follow our coding standards
4. **Test thoroughly** - Run pre-commit hooks
5. **Submit PR** - Include clear description

[Full Contributing Guide →](https://github.com/getaltair/altair/blob/main/CONTRIBUTING.md)

### Coding Standards
- ✅ Conventional commits
- ✅ Comprehensive tests
- ✅ Pre-commit hooks
- ✅ Keep-a-changelog format

---

## 💬 Community

**Get Support:**
- 🐛 [Report Issues](https://github.com/getaltair/altair/issues)
- 💬 [Discord Community](https://discord.gg/teuGe47Ufk)
- 📧 [Email Support](mailto:support@getaltair.com)

**Stay Updated:**
- 📖 [Changelog](https://github.com/getaltair/altair/blob/main/CHANGELOG.md)
- 🐦 [x](https://x.com/getaltair)
- 📝 [Blog](https://blog.getaltair.com) *(coming soon)*

---

## 📦 Repositories

### Main Repository
- [altair](https://github.com/getaltair/altair) - Monorepo for all apps

### Apps (in monorepo)
- `apps/altair_guidance` - Task management (✅ Implemented)
- `apps/altair-knowledge` - Personal wiki (📋 Phase 2)
- `apps/altair-tracking` - Inventory (📋 Phase 3)

### Shared Packages (in monorepo)
- `packages/altair-ui` - UI components & neo-brutalist theme
- `packages/altair-core` - Business logic, models, repositories
- `packages/altair-auth` - JWT authentication & token storage
- `packages/altair-sync` - PowerSync integration (📋 Planned)

### Backend Services (optional for sync)
- `services/auth-service` - FastAPI authentication server
- `services/ai-service` - AI provider proxy
- `services/sync-service` - PowerSync backend (📋 Planned)

---

## 📄 License

All Altair projects are licensed under **AGPL-3.0-or-later**

This means:
- ✅ Free to use, modify, distribute
- ✅ Must share modifications
- ✅ Network use = distribution (must share code)

[View License →](https://github.com/getaltair/altair/blob/main/LICENSE)

---

## 🌟 Philosophy

**Built for the ADHD community, by the ADHD community**

We believe:
- 🏠 **Local-first** - Your data belongs on your device
- ⚡ **Speed matters** - Friction kills momentum
- 🎯 **Focus is key** - One thing at a time, done well
- 🔐 **Privacy by default** - Sync is opt-in
- 🤝 **Open source** - Community-driven development

---

## ❤️ Acknowledgments

**Inspired by:**
- Local-first software principles
- The ADHD community's real needs
- Proven open-source tools
- [Minne](https://github.com/perstarkse/minne)

**Powered by:**
- Flutter - Cross-platform framework
- FastAPI - Modern Python web framework
- PowerSync - Offline-first sync engine

---

**Made with ☕ for people with ADHD**

*Status: 🚀 Phase 1 Complete - Beta Testing (Altair Guidance ready for download)*
