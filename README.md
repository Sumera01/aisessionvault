<div align="center">

<img src="https://img.shields.io/badge/version-1.0.0-7c6af7?style=flat-square" alt="version">
<img src="https://img.shields.io/badge/license-MIT-00d4c8?style=flat-square" alt="license">
<img src="https://img.shields.io/badge/zero%20dependencies-✓-34d16e?style=flat-square" alt="zero dependencies">
<img src="https://img.shields.io/badge/offline%20ready-✓-f5a623?style=flat-square" alt="offline ready">
<img src="https://img.shields.io/badge/deployed%20on-Vercel-000000?style=flat-square&logo=vercel" alt="Vercel">

<br /><br />

# 🔐 AI Session Vault

### Organize every AI conversation across every account.

A beautiful, zero-dependency, privacy-first app to track your AI chat sessions across ChatGPT, Claude, Gemini, Grok, Perplexity, DeepSeek, Copilot, and more — all stored locally in your browser.

**[→ Live Demo](https://aisessionvault.vercel.app)**

<br />

</div>

---

## ✨ Features

- **Multi-tool tracking** — Log sessions from ChatGPT, Claude, Gemini, Grok, Perplexity, DeepSeek, Copilot, and more
- **Multi-account support** — Separate work and personal accounts under one roof
- **Rich session cards** — Title, category, tool, account, chat link, notes, tags, and favorite status
- **Real-time search** — Instant search across title, category, account, notes, tags, and AI tool
- **Advanced filtering** — Filter by tool, category, account, or favorites — combinable with search
- **Smart sorting** — Newest, oldest, last updated, favorites first, or A–Z
- **Favorites system** — Star sessions to pin them for quick access
- **Analytics dashboard** — Visual breakdowns of sessions by tool, category, and account with animated charts
- **Import / Export** — Full JSON backup and restore with duplicate detection
- **Keyboard shortcuts** — `Ctrl+K` to search, `Ctrl+N` for a new session, `Esc` to close
- **Persistent storage** — IndexedDB keeps all data across refreshes, restarts, and reboots
- **100% private** — Nothing leaves your browser. No server, no telemetry, no tracking

---

## 🖼️ Screenshots

> Dashboard with session cards, stats, and sidebar tool filters

| Dashboard | New Session | Analytics |
|-----------|-------------|-----------|
| Stats, cards, search & filter | Quick-add form with tag input | Animated bar and donut charts |

---

## 🚀 Getting Started

### Option 1 — Use the hosted version

Just visit **[aisessionvault.vercel.app](https://aisessionvault.vercel.app)** — no install needed.

### Option 2 — Run locally

```bash
# Clone the repo
git clone https://github.com/yourusername/ai-session-vault.git
cd ai-session-vault

# Open the app — no build step required
open index.html
# or just double-click index.html in your file manager
```

### Option 3 — Self-host on Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/ai-session-vault)

---

## 📂 Project Structure

```
ai-session-vault/
└── index.html   ← The entire application (HTML + CSS + JS, self-contained)
```

That's it. One file. No build tools, no `node_modules`, no config files.

---

## 📋 Session Data Structure

Each session you save contains:

```json
{
  "id":          "unique identifier",
  "title":       "Session Title",
  "category":    "Bug Bounty",
  "aiTool":      "Claude",
  "account":     "personal@email.com",
  "chatLink":    "https://claude.ai/chat/...",
  "notes":       "Key findings and takeaways...",
  "tags":        ["xss", "bugbounty", "recon"],
  "createdDate": "2026-06-13T10:00:00.000Z",
  "lastUpdated": "2026-06-13T11:30:00.000Z",
  "favorite":    false
}
```

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + K` | Focus search |
| `Ctrl + N` | New session |
| `Ctrl + 1` | Go to Sessions |
| `Ctrl + 2` | Go to Favorites |
| `Ctrl + 3` | Go to Analytics |
| `Esc` | Close modal |

---

## 💾 Data & Privacy

All data is stored in your browser's **IndexedDB** — a persistent, structured local database. It survives:

- Browser refresh
- Browser restart
- Computer restart

**Nothing is ever sent to a server.** There is no backend, no account, no sync, and no analytics on your usage. Your sessions are yours.

To move data between devices, use **Settings → Export Backup** to download a `sessions.json` file, then **Import Backup** on another device.

---

## 🛠️ Tech Stack

| Layer | Choice | Why |
|-------|--------|-----|
| Storage | IndexedDB | Persistent, structured, works offline |
| Styling | Pure CSS with variables | Zero dependencies, fast |
| Logic | Vanilla JavaScript (ES2020+) | No framework overhead |
| Charts | Pure SVG + JS | No chart library needed |
| Deployment | Vercel (static) | One file, instant deploys |

---

## 🗂️ Suggested Categories

The app supports any custom category. Here are some to get you started:

`Bug Bounty` · `Cybersecurity` · `AI` · `Machine Learning` · `Deep Learning` · `College` · `Startup` · `Programming` · `Research` · `Personal`

---

## 📤 Import / Export

**Export:** Go to **Settings & Backup → Download sessions.json**. This creates a timestamped JSON file with all your sessions.

**Import:** Go to **Settings & Backup → Import sessions.json** and select a previously exported file. Duplicates are automatically detected and skipped — no data loss.

The export format is a plain JSON object:

```json
{
  "version": 1,
  "exportedAt": "2026-06-13T12:00:00.000Z",
  "sessions": [ ...your sessions... ]
}
```

---

## 🤝 Contributing

Contributions are welcome. Since the entire app is a single HTML file, there's no build step to worry about.

1. Fork the repo
2. Edit `index.html`
3. Open it in your browser to test
4. Submit a pull request

Please keep the zero-dependency philosophy intact.

---

## 📜 License

MIT — do whatever you want with it.

---

<div align="center">

Built with pure HTML, CSS, and JavaScript · No frameworks · No tracking · No nonsense

**[aisessionvault.vercel.app](https://aisessionvault.vercel.app)**

</div>
