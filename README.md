# Awesome-Rich-Text-Editing-Document-Authoring

# Awesome Rich Text Editing & Document Authoring

> A curated list of top Rich Text Editing and Document Authoring platforms — both SaaS/Hosted commercial solutions and open-source alternatives for collaborative writing, formatting, and structured content creation.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Google Docs](#google-docs)
  - [Microsoft Word Online](#microsoft-word-online)
  - [Notion](#notion)
  - [Coda](#coda)
  - [Quip](#quip)
  - [Dropbox Paper](#dropbox-paper)
- [Open-Source Software](#-open-source-software)
  - [Nextcloud Write](#nextcloud-write)
  - [La Suite Docs](#la-suite-docs)
  - [AFFiNE](#affine)
  - [Alexandrie](#alexandrie)
  - [Libera Words](#libera-words)
  - [LyX](#lyx)
  - [TypstPad](#typstpad)
  - [Papyrus](#papyrus)
  - [Periwiki](#periwiki)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Rich Text Editing and Document Authoring platforms. These are not open-source but are included as reference points for feature comparison.

### Google Docs
**Type:** Real-time collaborative document editing  
Google Docs is the most widely adopted cloud document editor, offering real-time co-editing with live cursors, comments, suggestions, and deep integration with Google Workspace. It supports DOCX/ODT compatibility and is the default choice for teams already in the Google ecosystem.

### Microsoft Word Online
**Type:** Browser-based Word with Office compatibility  
Word Online provides the familiar Microsoft Word experience in the browser, with real-time co-authoring, comments, and track changes. It is the natural choice for organizations standardized on Microsoft 365, with seamless transition to desktop Word for advanced formatting.

### Notion
**Type:** Flexible workspace with block-based editing  
Notion combines rich text editing with databases, wikis, and project management in a highly flexible block-based workspace. Its strength is freedom: teams can build documents, tables, and knowledge bases without rigid structures. The trade-off is that governance requires team conventions to prevent fragmentation.

### Coda
**Type:** Doc-based workspace with tables and automation  
Coda combines documents, spreadsheets, and automation into a single canvas. Teams can build custom workflows and trackers within a doc-like interface, positioned for teams wanting more structured data capabilities than Notion provides.

### Quip
**Type:** Collaborative documents within Salesforce ecosystem  
Quip (Salesforce) provides collaborative documents and spreadsheets with integrated chat and comments. It is the natural choice for Salesforce customers wanting document collaboration tied to CRM records.

### Dropbox Paper
**Type:** Collaborative docs integrated with Dropbox  
Dropbox Paper provides collaborative document editing with a clean, minimalist interface, integrated with Dropbox storage. Suited for teams already using Dropbox for file storage wanting lightweight document collaboration.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Rich Text Editing and Document Authoring tools. The open-source ecosystem spans **full office suites**, **Notion-style block editors**, **Markdown-based note tools**, and **specialized document processors**.

### Nextcloud Write
**Stack:** PHP / Collabora or Euro-Office | **License:** AGPL-3.0  
Nextcloud Write is a full-featured, real-time collaborative document editor that runs entirely on infrastructure of your choice, positioned as a sovereign open-source alternative to Word and Google Docs [citation:1]. Key features include:
- **Real-time co-editing** with colored cursors and a formal review mode for tracking edits and accepting/rejecting changes
- **Granular sharing** via internal permissions or public links, with support for read-only, editable, or watermarked access
- **Federated collaboration** allowing teams on separate Nextcloud instances to co-author the same document across servers
- **Automatic saving and version history**, with compare-and-combine tools for reconciling divergent versions
- **DOCX and ODT support**, ensuring documents remain intact across software
- **Offline editing** with sync on reconnection
- **AI assistant integration** via Nextcloud Assistant, with administrator control over whether the model runs locally or on a trusted provider

Deploys as part of Nextcloud Office, which also includes spreadsheet and presentation editors [citation:1].  
**Best for:** Organizations wanting a complete, self-hosted document suite with real-time collaboration, federation, and full data sovereignty, particularly those already running Nextcloud.

### La Suite Docs
**Stack:** Django / Next.js / ProseMirror / Yjs | **License:** MIT  
La Suite Docs is an open-source collaborative editor positioned as a sovereign alternative to Notion or Google Docs, backed by the German Center for Digital Sovereignty (ZenDiS) and the French DINUM [citation:8][citation:15]. Key features include:
- **Rich-text and Markdown editing** with slash commands and a block system
- **Real-time collaboration** with live cursors, presence, comments, and granular access control
- **Subpages and hierarchy** for knowledge organization, with searchable content
- **Import/export** to `.docx` and `.md`, with export to `.docx`, `.odt`, and `.pdf`
- **Offline editing** and optional AI writing helpers (rewrite, summarize, translate, fix typos)

Version 5.0.0 separated document content and metadata in the API, with dedicated endpoints for reading and writing content, and added Mistral AI integration alongside OpenAI [citation:8]. Self-hosting supports Kubernetes, Docker Compose, and community methods like Nix and YunoHost. **Note:** Some advanced features (e.g., PDF export) rely on GPL-licensed BlockNote packages; you can build without them using `PUBLISH_AS_MIT=true` [citation:15].  
**Best for:** Public institutions, companies, and open communities wanting a Notion/Google Docs alternative with strong European sovereignty backing and block-based editing.

### AFFiNE
**Stack:** TypeScript / Rust (OctoBase) | **License:** MIT (Community Edition)  
AFFiNE is a free, open-source, self-hostable knowledge base that integrates block documents and an infinite canvas, allowing users to organize documents and databases like Notion while arranging diagrams and sticky notes on a free canvas like Miro [citation:9]. Key features include:
- **Seamless switching** between document editing and edgeless canvas for diagrams, mind maps, and sticky notes
- **AI-powered creation support** (writing, slides, summarization) configurable with your own API keys or local LLMs
- **Offline use and synchronization** via local storage, with sync to self-hosted servers
- Cross-platform clients for Windows, macOS, iOS, and Android

Self-hosting via Docker Compose is documented, with a straightforward setup process [citation:9]. The Community Edition is MIT-licensed and self-hostable, with AI features available by configuring your own provider keys.  
**Best for:** Teams wanting a unified document + whiteboard workspace with MIT licensing, particularly those who need visual planning alongside written knowledge.

### Alexandrie
**Stack:** Vue/Nuxt / Go / MySQL / S3 | **License:** Open Source  
Alexandrie is an open-source note-taking app that keeps your data at home, positioned as a privacy-respecting alternative to Notion or Evernote [citation:2]. Key features include:
- **Enhanced Markdown editor** with organization by workspaces, categories, and tags
- **Fast search** and clean interface, with export to PDF or Markdown
- **Offline support** via PWA technology
- **Permissions system** for sharing notes with view/edit controls
- **Standard Markdown storage**, making migration to other apps straightforward

Runs on Vue/Nuxt frontend and Go backend with MySQL and S3-compatible storage. Deployment via Docker Compose [citation:2].  
**Best for:** Individuals and small teams wanting a self-hosted, Markdown-based note-taking app with data sovereignty and a modern interface, accepting a lighter feature set than Notion.

### Libera Words
**Stack:** Python / Euro-Office (AGPL fork of ONLYOFFICE) | **License:** AGPL-3.0  
Libera Words is part of Libera Suite, a desktop office suite that opens `.docx`, `.odt`, `.rtf`, `.txt`, and `.md` files, edits them locally, and saves them back without requiring an account or phoning home [citation:4]. Key characteristics:
- **Four editors** (Words, Tables, Slides, Diagrams) share one application, with the file type selecting the editor automatically
- **Runs locally** using the system's webview, with editors served over a loopback HTTP server
- **Builds from pinned upstream sources**, with a patch queue that does not touch the editing engine
- **Early-stage**: works on macOS (Apple Silicon) and Linux (x86_64 and arm64); Windows not yet started

**Important:** This is a **desktop application**, not a web-based collaborative editor. It prioritizes local ownership and offline editing over real-time collaboration [citation:4].  
**Best for:** Users wanting a local-first desktop office suite with document compatibility and no cloud dependency, accepting that it is early-stage and lacks collaboration features.

### LyX
**Stack:** C++ / Qt | **License:** GPL  
LyX is a document processor that encourages writing based on document structure (WYSIWYM) rather than appearance (WYSIWYG) [citation:11]. It combines the power of TeX/LaTeX with a graphical interface, offering:
- **World-class support for mathematical content** via a fully integrated equation editor
- **Structured documents** for academic articles, theses, books, and scripts
- **Reference list and index creation** as standard features
- **Broad array of pre-designed document layouts** built in

LyX looks like a word processor on screen, but its printed output—or richly cross-referenced PDF—reflects the underlying structural markup [citation:11]. Recent releases include LyX 2.5.1 (April 2026).  
**Best for:** Academics, scientists, and technical writers wanting structured, high-quality document output with LaTeX power without writing LaTeX directly.

### TypstPad
**Stack:** Go / Typst / Yjs | **License:** Open Source  
TypstPad is a self-hosted collaborative Typst document editor positioned as "Overleaf for Typst" [citation:12]. Key features include:
- **Real-time collaboration** with live cursors and presence (Yjs CRDT)
- **Live preview** with Typst compiled to WASM, errors shown with click-to-jump, and fonts/packages served by your own server
- **SSO** via generic OIDC (Keycloak, Authentik, Google, Azure AD) plus built-in accounts
- **Version history** with automatic snapshots, named versions, visual diffs, and one-click restore
- **Suggestions mode** for tracked changes, and threaded comments anchored to text ranges
- **AI integration** via REST API, MCP server, and CLI for agents like Claude to read, edit, suggest, and compile
- **PDF export** in-browser or server-side

Deploys via Docker Compose with a straightforward setup [citation:12].  
**Best for:** Technical teams writing structured or scientific documents wanting a collaborative, self-hosted editor with Typst's typesetting power and modern AI integration.

### Papyrus
**Stack:** Go / JavaScript | **License:** BSD-3-Clause  
Papyrus is a real-time collaborative Markdown editor and document repository with simple organization and project-based management [citation:5]. Core features include:
- **Collaborative editing** via operational transformation
- **Organizations and projects** for document grouping
- **Google or GitHub login** for authentication
- **Docker Compose deployment** with a simple setup

**Important:** Papyrus was built during GopherGala 2016, and the README notes that some functionality (member removal, document deletion) is lacking [citation:5]. Evaluate maintenance status before production use.  
**Best for:** Developers wanting a simple, self-hosted collaborative Markdown editor with project organization, accepting that the project is dated and may require customization.

### Periwiki
**Stack:** Go / SQLite | **License:** Open Source  
Periwiki is a self-hosted wiki for people who miss the old web, described as MediaWiki-inspired and Goldmark-powered with no JavaScript [citation:6]. Features include:
- **CommonMark extended with WikiLinks** (`[[Wikilink]]` syntax)
- **Full revision history** with diffs between any two versions
- **User accounts** with optional anonymous editing
- **Self-contained binary** with SQLite, running instantly

It is a **wiki engine** rather than a rich text editor—content is authored in Markdown, and the focus is on simple, cache-friendly server-rendered HTML [citation:6].  
**Best for:** Individuals and small teams wanting a lightweight, no-JavaScript wiki for personal knowledge bases or passion projects, accepting a Markdown-only authoring model.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Real-Time Collab | Block/Canvas | Self-Hosted | Best For |
|----------|---------|-------|------------------|--------------|-------------|----------|
| **Google Docs** | Proprietary | Cloud | ✅ | ❌ | ❌ | Universal collaboration |
| **Microsoft Word Online** | Proprietary | Cloud | ✅ | ❌ | ❌ | Microsoft 365 estates |
| **Notion** | Proprietary | Cloud | ✅ | ✅ Blocks + DB | ❌ | Flexible workspace |
| **Nextcloud Write** | AGPL-3.0 | PHP/Collabora | ✅ | ❌ | ✅ | Full office suite + federation |
| **La Suite Docs** | MIT | Django/Next.js | ✅ | ✅ Blocks | ✅ | Sovereign Notion alternative |
| **AFFiNE** | MIT (CE) | TS/Rust | ✅ | ✅ Docs + canvas | ✅ | Unified docs + whiteboard |
| **Alexandrie** | Open Source | Vue/Go | (Permissions) | ❌ Markdown | ✅ | Privacy-first note-taking |
| **Libera Words** | AGPL-3.0 | Python/Euro-Office | ❌ (Desktop) | ❌ | ✅ (Local) | Local-first desktop suite |
| **LyX** | GPL | C++/Qt | ❌ | ❌ (Structured) | ✅ (Desktop) | Academic/technical authoring |
| **TypstPad** | Open Source | Go/Typst | ✅ | ❌ | ✅ | Collaborative Typst editor |
| **Papyrus** | BSD-3-Clause | Go/JS | ✅ | ❌ | ✅ | Simple Markdown collab (dated) |
| **Periwiki** | Open Source | Go/SQLite | ❌ (Wiki) | ❌ | ✅ | Lightweight Markdown wiki |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Rich Text Editing or Document Authoring tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem **splits** between **full office suites with real-time collaboration** (Nextcloud Write, La Suite Docs, AFFiNE), **Markdown-based note tools** (Alexandrie, Papyrus, Periwiki), **local-first desktop applications** (Libera Words, LyX), and **specialized document processors** (TypstPad for Typst, LyX for LaTeX-structured authoring). **Nextcloud Write** is the most complete open-source replacement for Google Docs/Word with federation and data sovereignty [citation:1], while **La Suite Docs** offers the strongest Notion-style block editing with government-backed European sovereignty [citation:8][citation:15]. **AFFiNE** uniquely combines documents and whiteboard canvas in one workspace [citation:9].

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
