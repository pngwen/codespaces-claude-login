# 🤖 Codespaces Claude Login Helper

> **🌐 Live App:** [https://pngwen.github.io/codespaces-claude-login](https://pngwen.github.io/codespaces-claude-login)

A simple, single-page web app that walks you through authenticating **Claude Code** inside a GitHub Codespace — no backend required, pure vanilla JavaScript.

## 🤔 Why Does This Exist?

Claude Code's OAuth flow expects to redirect back to `localhost`, but inside a Codespace your dev environment lives in the cloud. The redirect fails because there's no real `localhost` — only a forwarded port URL. This tool bridges that gap by helping you construct the correct callback URL manually.

## 🚀 How It Works

The app guides you through a step-by-step process:

1. **📋 Install Claude Code** — Shows you the `curl` install command, ready to copy.
2. **🔗 Paste your Auth URL** — Paste the OAuth URL that Claude Code gives you. The app extracts the port number from the `redirect_uri` automatically.
3. **🌍 Enter your Port Forwarding URL** — Paste the Codespaces forwarding URL for that port.
4. **✅ Authorize Claude Code** — Click the generated link to open the OAuth page in a new tab.
5. **🔁 Paste the Failed Redirect URL** — After auth, the browser will land on a broken URL. Paste it here.
6. **🎯 Get the Fixed URL** — The app swaps `localhost` for your forwarding URL and gives you the correct callback link to click.
7. **🎉 Done!** — If you see "Build something great", you're authenticated!

## 🛠️ Tech Stack

- Pure **vanilla JavaScript** — zero dependencies, zero build steps
- Single file: `index.html`
- Works entirely in the browser on the client side.

## 📄 License

See [LICENSE](LICENSE).

---

> 🍴 Forked and extended with ❤️ — contributions welcome!

---

© 2026 [Robert Lowe (pngwen)](https://github.com/pngwen) — Released under the [MIT License](LICENSE)
