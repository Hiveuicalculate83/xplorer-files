<div align="center">

<img height="120" src="apps/src-tauri/icons/icon.png" alt="Xplorer" />

<h1>Xplorer File Manager</h1>

<p><strong>A customizable, modern file manager built with Rust, React, and Tauri.</strong></p>

<p>
Cross-platform file browsing, AI-assisted workflows, extensibility, Git tools, previews, themes, and multi-pane productivity in one desktop application.
</p>

<p>
<a href="https://xplorer.space">Website</a> ·
<a href="https://xplorer.space/docs">Documentation</a> ·
<a href="https://github.com/kimlimjustin/xplorer/discussions">Discussions</a>
</p>

</div>

---

## 📌 Overview

Xplorer is a modern desktop file manager designed for users who want more than basic folder navigation. It combines a Rust backend with a React frontend through Tauri 2, aiming to provide a flexible, cross-platform file management experience for Windows, macOS, and Linux.

The project focuses on practical file workflows: browsing folders, previewing files, managing archives, working with tabs and split panes, using keyboard-driven navigation, and organizing files through a customizable interface. Xplorer also includes AI-assisted features, Git integration, an extension system, themes, and developer-oriented tooling.

This codebase represents the `next` branch, described as a full rewrite using Tauri 2, React 18, and a new extension system. It is actively developed and is not described as production-ready.

## ✨ Key Features

### 📁 File Management

Xplorer provides a desktop file management interface with multiple ways to browse and organize files.

- Cross-platform support for Windows, macOS, and Linux
- Multiple view modes:
  - Grid
  - List
  - Details
  - Column
  - Gallery
  - Tree
- Multi-tab browsing
- Split panes
- Session persistence
- Archive support for ZIP, TAR, GZ, BZ2, and XZ
- Password-protected archive support
- File operations designed around memory-mapped I/O and parallel chunked transfers

### 🤖 AI-Assisted Workflows

Xplorer includes AI integration for users who want file-aware assistance while working with documents, code, and other local content.

Supported AI provider categories listed in the project include:

- OpenAI
- Anthropic
- Google
- DeepSeek
- Mistral
- Ollama

AI-related capabilities described by the project include:

- AI chat with file context awareness
- Natural language file search
- Fuzzy file search
- Semantic file search
- Smart categorization
- Agentic file operations

### 🧑‍💻 Developer Tools

Xplorer is also designed for software development workflows where files, Git history, terminal access, and previews are frequently used together.

Developer-focused features include:

- Git integration
  - Branches
  - Staging
  - Commits
  - Diffs
  - Blame
  - Stash
- Integrated terminal
- SSH remote browsing
- Command palette
- Configurable keyboard shortcuts
- Rich previews for:
  - Code with syntax highlighting
  - Markdown
  - PDF
  - Word documents
  - Spreadsheets
  - Audio
  - Video

### 🧩 Extensibility and Customization

Xplorer is designed to be customizable through extensions, themes, and configurable workflows.

Extension and customization features described by the project include:

- Extension marketplace at `xplorer.space`
- Public extension SDK
- Sandboxed extension runtime
- Built-in extension categories such as:
  - Git UI
  - SSH manager
  - Docker
  - Google Drive
  - Code editor
  - Image editor
  - File hasher
- Theme support, including:
  - Tokyo Night
  - Dracula
  - Nord
  - Cyberpunk
  - Ocean Deep

## 🧭 Use Cases

### For Developers

Xplorer can be used as a file manager for development work where repository navigation, Git state, file previews, and terminal access are part of the same workflow. Split panes and multi-tab browsing are useful when comparing folders, moving between project areas, or reviewing related files side by side.

Git integration makes it possible to work with branches, staged changes, commits, diffs, blame information, and stashes from within the file management environment.

### For Researchers and Students

For document-heavy workflows, Xplorer’s AI chat and semantic search features are intended to help users work with file content more naturally. Instead of relying only on exact filenames, users can search by meaning, ask questions about documents, and summarize or inspect file context through AI-assisted workflows.

This makes the project relevant for users managing notes, papers, reports, coursework, references, and collections of mixed document formats.

### For Power Users

Xplorer includes features commonly associated with advanced desktop productivity: a command palette, configurable shortcuts, multiple view modes, split panes, tabs, session persistence, and per-workflow customization through themes and extensions.

These capabilities are useful for users who frequently move files, organize large folders, compare directories, preview many file types, and prefer keyboard-driven workflows.

## 🏗️ Technology Stack

| Layer | Technology |
|---|---|
| Desktop framework | Tauri 2 |
| Backend | Rust |
| Async/runtime tooling | Tokio |
| Parallel processing | Rayon |
| Frontend | React 18 |
| Language | TypeScript |
| Styling | Tailwind CSS |
| Build tool | Vite |
| Marketplace web app | Next.js |
| Database tooling | Prisma |
| Payments referenced by project | Stripe |
| End-to-end testing | Playwright |
| Frontend testing | Vitest |

## 🛠️ Development

The project README describes the following development requirements:

- Node.js 20+
- pnpm 10+
- Rust latest stable via `rustup`

Development commands provided by the project:

```bash
git clone https://github.com/kimlimjustin/xplorer.git -b next
cd xplorer
pnpm install
pnpm dev:app
```

The project also documents these commands:

```bash
pnpm build
pnpm test
pnpm run test:tauri
```

The full stack development workflow, including the marketplace web server, is documented as using:

```bash
pnpm dev
```

The marketplace workflow is described as requiring local PostgreSQL via:

```bash
pnpm run marketplace:db
```

## 🧱 Architecture Summary

Xplorer is organized as a desktop application with a frontend, backend, marketplace, SDK packages, extensions, tests, infrastructure, and scripts.

The main parts described by the project are:

- React 18 + TypeScript + Vite desktop frontend
- Rust backend using Tauri 2
- Next.js marketplace web application
- Internal service-layer SDK
- Public extension SDK
- Extension scaffolding package
- Built-in extension packages
- Playwright end-to-end tests
- Docker Compose infrastructure for PostgreSQL
- Extension signing utilities

## 🧪 Project Status

The project README identifies this as the `next` branch and describes it as a full rewrite using Tauri 2, React 18, and a new extension system.

It is also explicitly described as:

- Actively developed
- Not yet production-ready
- Open to feedback

## 🙋 FAQ

### Is Xplorer a standard file manager?

Xplorer is a file manager, but it is designed to include more than basic folder browsing. It combines traditional file management with AI-assisted search, Git tools, file previews, extensions, themes, tabs, split panes, and developer-focused workflows.

### What platforms are listed for Xplorer?

The project describes Xplorer as cross-platform and lists Windows, macOS, and Linux.

### Does Xplorer include AI features?

Yes. The project describes AI chat, file context awareness, natural language search, fuzzy search, semantic search, smart categorization, and support for connecting AI providers through APIs.

### Is Xplorer production-ready?

The project README states that the `next` branch is not yet production-ready and is actively developed.

### Can Xplorer be extended?

Yes. The project describes a new extension system, a public extension SDK, a sandboxed runtime, and an extension marketplace.

### What license does Xplorer use?

Xplorer is licensed under AGPL-3.0.

## 🤝 Contributing

Contributions are welcome according to the project documentation. For setup and contribution guidelines, see `CONTRIBUTING.md`.

Useful community entry points include:

- Bug reports through GitHub Issues
- Feature discussion through GitHub Discussions

## 📄 License

Xplorer is licensed under the [AGPL-3.0](LICENSE).
