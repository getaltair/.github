# Altair

> ADHD-friendly productivity ecosystem that works offline-first

[![License](https://img.shields.io/badge/license-AGPL--3.0-blue.svg)](https://github.com/getaltair/altair/blob/main/LICENSE)
[![Flutter](https://img.shields.io/badge/Flutter-3.0+-02569B?logo=flutter)](https://flutter.dev)
[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?logo=python)](https://python.org)
[![Status](https://img.shields.io/badge/status-Phase%201%20Development-yellow)]()

---

## 🎯 What We're Building

**Three focused apps for ADHD project management:**

1. **🎯 Guidance** - Task & project management (Building now)
2. **📚 Knowledge** - Personal wiki & notes (Coming Month 4)
3. **📦 Tracking** - Inventory & resources (Coming Month 7)

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

### 🎯 Altair Guidance (Phase 1: Now)
**Task and project management for ADHD**

**Core features:**
- Quick capture (< 3 seconds)
- AI-powered task breakdown
- Visual time tracking
- Offline-first with optional sync

**Status:** ✅ Month 1 complete (Infrastructure)
**Next:** Month 2 - Core task management

[View Guidance README →](https://github.com/getaltair/altair/tree/main/apps/altair-guidance)

### 📚 Altair Knowledge (Phase 2: Month 4-6)
**Personal wiki and knowledge management**

**Planned features:**
- Markdown-based notes
- Automatic backlinks & graph view
- Daily notes
- Cross-app linking with Guidance

**Status:** 📋 Planned for Month 4

### 📦 Altair Tracking (Phase 3: Month 7-9)
**Inventory and resource management**

**Planned features:**
- Barcode scanning
- Location-based organization
- Smart alerts (low stock, expiration)
- Integrates with tasks and wiki

**Status:** 📋 Planned for Month 7

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

**Phase 1: Altair Guidance** (Months 1-3)

- ✅ Month 1: Foundation complete
  - CI/CD pipeline
  - Project structure
  - Authentication foundation
  - Neo-brutalist UI theme

- ⏳ Month 2: Core features (In Progress)
  - Task management
  - Quick capture
  - Local storage

- 📋 Month 3: AI & polish (Planned)
  - AI task breakdown
  - Beta testing
  - Performance optimization

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
- 💬 [Discord Community](https://discord.gg/altair)
- 📧 [Email Support](mailto:support@getaltair.com)

**Stay Updated:**
- 📖 [Changelog](https://github.com/getaltair/altair/blob/main/CHANGELOG.md)
- 🐦 [x](https://x.com/getaltair) *(coming soon)*
- 📝 [Blog](https://blog.getaltair.com) *(coming soon)*

---

## 📦 Repositories

### Main Repository
- [altair](https://github.com/getaltair/altair) - Monorepo for all apps

### Apps (in monorepo)
- `apps/altair-guidance` - Task management
- `apps/altair-knowledge` - Personal wiki (Phase 2)
- `apps/altair-tracking` - Inventory (Phase 3)

### Shared Packages (in monorepo)
- `packages/altair-ui` - UI components & theme
- `packages/altair-core` - Business logic
- `packages/altair-auth` - Authentication
- `packages/altair-sync` - Sync engine integration

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

*Status: 🚧 Phase 1 Development (Month 1 Complete)*
