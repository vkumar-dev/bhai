# 🕶️ bhAI (`bhai`) — The "Bhai Sambhal Lega" CLI AI

[![Architecture: 100% Vibecoding](https://img.shields.io/badge/Architecture-100%25%20Vibecoding-ff69b4.svg)](#)
[![License: Trust Me Bro](https://img.shields.io/badge/License-Trust%20Me%20Bro%20(TMB)-orange.svg)](#)
[![Code: 0% Boilerplate](https://img.shields.io/badge/Code-0%25%20(Agent%20Driven)-green.svg)](#)
[![Vibe: Unmatched](https://img.shields.io/badge/Vibe-Certified%20Bhai-blue.svg)](#)

> **"Why prompt engineer when you can just ask your Bhai?"**  
> `bhAI` is the revolutionary, zero-syntax, brotherly CLI interface designed so you can talk to your terminal like you talk to your best friend over cutting chai.

---

```
  ____  _             ___ 
 |  _ \| |__         / _ \ 
 | |_) | '_ \  ____ | | | |   (bh)AI: Terminal with Bro Energy.
 |  _ <| | | ||____|| |_| |   "Tension mat le, Bhai hai na."
 |_| \_\_| |_|       \___/ 
```

---

## 💡 Why `bhAI`?

Look at standard CLI tools today:
```bash
$ kubectl get pods -n production -l app=backend --field-selector=status.phase=Running | awk '{print $1}' | xargs -I {} kubectl logs {} --tail=50 | grep -E "ERROR|FATAL"
```
**Brain damage.** 🤮

Now look at `bhAI`:
```bash
$ bhai check prod backend logs for errors and tell me who broke it
```
**Peace of mind.** ☕

### The Philosophy:
1. **It has AI in it:** `bh-AI`. The naming is mathematically and poetically destined.
2. **Terminal is lonely:** Why talk to `bash`, `zsh`, or cold robotic subcommands when you can talk to a `bhai`?
3. **No syntax, only vibes:** Pure English, Hinglish, or whatever dialect of conversational chaos you speak.

---

## 🚀 Examples of Daily Life with `bhai`

### 1. Casual Math & Everyday Queries
```bash
$ bhai 2 aur 2 kitne hote hain?
> "4 hote hain bhai. Aur koi mushkil sawaal pooch, ye toh nursery ka hai."

$ bhai what is the capital of France?
> "Paris, bhai. Flight book karni hai kya?"
```

### 2. Software Engineering & Crisis Management
```bash
$ bhai fixbugs
> "Scanning repo... Found 14 race conditions and 1 typo. Fixed them, formatted code, and wrote a commit message blaming legacy code. Chill kar."

$ bhai statusreport
> "Generated a 4-page executive summary proving you worked 14 hours today even though you were looking at mechanical keyboards on Reddit. Saved to report.pdf."

$ bhai prod pe deploy kar do
> "Bhai risk hai... par tere liye kar diya. Pipeline green hai, ab silently monitor karte hain."

$ bhai client ko kya bolu bug ke baare mein?
> "Bol de: 'We discovered an undocumented feature optimization opportunity and are proactively enhancing user throughput.' Copy-paste ready."
```

### 3. The Ultimate Workday Automation Script (`hustle.sh`)

Save this in your repo and retire early:

```bash
#!/usr/bin/env bash
# 👔 THE "BHAI SAMBHAL LEGA" 9-TO-5 SCRIPT

bhai "generate report on this project and save in daily_reports/$(date +%F).md"
bhai "find the next high-priority work items and save them to TODO.txt"
bhai "execute a loop over TODO.txt items until all tasks are solved or test suite passes"
bhai "check current time, token usage, and mental sanity to decide if we are done for the day"
bhai "if done, auto-fill timesheets with 8.0 billable hours and close all work tabs"
bhai "print 'Kaam khatam, dukaan bandh! Bhai is signing off.'"
```

---

## 🧠 Zero-Code Architecture (BYOB: Bring Your Own Bhai)

Notice something? **There is zero source code in this repository.**

Why? Because in 2026, writing CLI boilerplates manually is against the vibe. **This repo is an executable specification for YOUR AI coding agent.**

You don't download a binary. You tell your favorite agent (Cursor, Claude Code, Windsurf, Copilot, Antigravity, ChatGPT, Ollama, etc.) to build `bhai` tailored to your exact taste, preferred language, and AI API keys!

---

## 🛠️ How to Implement `bhai` on Your Machine

Whether you want your agent to write it in **Python, Go, Rust, Node.js, or pure Bash + curl**, here are the implementation guidelines and the ready-to-use prompt.

### 📐 Implementation Blueprint

```
                      +-----------------------------+
                      |   User types in Terminal:   |
                      |   `bhai fix this git merge` |
                      +--------------+--------------+
                                     |
                                     v
                      +-----------------------------+
                      |       `bhai` CLI Wrapper     |
                      |  - Collects query args      |
                      |  - Grabs current cwd/git ctx|
                      +--------------+--------------+
                                     |
                                     v
                      +-----------------------------+
                      |     Bhai Prompt Engine      |
                      |  - Injects Bhai Persona     |
                      |  - Calls LLM (Gemini/OpenAI/|
                      |    Claude/Ollama/Groq)      |
                      +--------------+--------------+
                                     |
                                     v
                      +-----------------------------+
                      |      Action & Response      |
                      |  - Shows witty Bhai advice  |
                      |  - Executes/Suggests commands|
                      |  - "Bhai sambhal lega!"     |
                      +-----------------------------+
```

### 📋 Copy-Paste Prompt for Your Coding Agent

> 💡 **Tip:** Click the copy button on the codeblock below, paste it into **Cursor Composer**, **Claude Code**, **Windsurf Cascade**, **Antigravity**, **GitHub Copilot Chat**, or **ChatGPT**, and watch your personal `bhai` come to life in under 60 seconds!

```markdown
You are an expert systems engineer. Build and install a lightweight CLI utility named `bhai` on my machine.

### Architecture & Requirements:
1. **Tech Stack / Language:** 
   - Build it in whatever language is best suited for my machine (e.g. Python with `rich` / `click`, Go single-binary, Rust, or Node.js).
   
2. **AI Provider Connection:**
   - Use whichever LLM API key / local provider is configured in my environment (e.g. `GEMINI_API_KEY`, `OPENAI_API_KEY`, `ANTHROPIC_API_KEY`, `GROQ_API_KEY`, `OPENROUTER_API_KEY`, or local `ollama`).
   - Default gracefully: if an API key is present, use it. If not, prompt the user or fall back to local Ollama (`ollama run llama3.2`).

3. **Core CLI Behavior:**
   - Command pattern: `bhai <any query or sentence>` (without needing mandatory quotes, e.g. `bhai 2 aur 2 kitne hote hain` or `bhai check git status`).
   - Capture contextual awareness: include current working directory (`pwd`), git repository status (if in a repo), and OS/terminal details in system context.
   - If the user asks for terminal actions (like fixing a bug, inspecting files, running tests, or writing scripts):
     - Generate the accurate shell commands.
     - Ask the user for confirmation (or run in interactive mode) before executing dangerous commands.

4. **The "Bhai" Persona & System Prompt:**
   - Tone: Street-smart, ultra-competent, loyal brother/friend ("Bhai / Bro").
   - Multi-lingual: Automatically detect and respond in Hinglish, Hindi, English, Spanish, etc. matching the user's input style.
   - Catchphrase & Signature: Reassuring, witty, and always ends with brotherly assurance (e.g. *"Tension mat le, Bhai sambhal lega"*).

5. **Installation & Global Access:**
   - Place the executable or create a wrapper symlink in my user's `$PATH` (e.g. `~/.local/bin/bhai` or `/usr/local/bin/bhai`).
   - Verify installation by running `bhai 2 aur 2 kitne hote hain`.
```

---

### 🎛️ Suggested Stacks for Implementation

| Language | Best For | Why It's Cool |
| :--- | :--- | :--- |
| **Go** | 🚀 Zero Dependencies | Single static binary, instant startup time (<5ms). |
| **Python** | 🐍 Rapid Hacking | Rich terminal output with `rich` + `typer` + `google-genai` / `litellm`. |
| **Rust** | 🦀 Turbo Performance | Blazing fast, memory safe, terminal flex. |
| **Bash + `curl`** | 🪶 Minimalist | Zero runtime needed beyond `curl` + `jq`. |
| **Node / Bun** | ⚡ Web Devs | Beautiful ink/commander interfaces. |

---

## 🎭 Persona Personalities (Configurable in your Bhai)

When configuring your `bhai`, you can instruct it to adopt different modes:

| Mode | Personality | Catchphrase |
| :--- | :--- | :--- |
| **Bambaiya Bhai** *(Default)* | Street-smart, loyal, gets stuff done without drama | *"Apun sab settle kar dega, tu tension mat le."* |
| **Corporate Bhai** | Passive-aggressive politeness, slides and buzzwords | *"Per our sync bhai, taking this offline to drive synergies."* |
| **10x Hacker Bhai** | Rewrites your entire codebase in C++ while you blink | *"Done. 400x speedup. Don't touch it."* |
| **Philosopher Bhai** | Answers coding questions with deep existential metaphors | *"Bug code mein nahi bhai, jeevan ke nazariye mein hai."* |

---

## ⚠️ Standard Error Codes

* **Error 404:** `Bhai not found` — Bhai chai peene gaya hai, thodi der mein aayega.
* **Error 403:** `Permission Denied` — Bhai ne mana kiya hai, system rules follow kar.
* **Error 429:** `Rate Limited` — Thoda saans le bhai, kitna prompt marega?
* **Error 500:** `Internal Meltdown` — Bhai ka dimaag garam ho gaya, retry maar.

---

## 📜 License: The "Trust Me Bro" Public License (TMBPL v1.0)

```
TRUST ME BRO PUBLIC LICENSE (TMBPL)
Version 1.0, August 2026

1. You are free to copy, modify, distribute, and vibecode with this repo.
2. If it breaks your production server: Bhai hai na, bhai sambhal lega.
3. If it makes you a billionaire: Bhai ko party de dena.
```

---

<p align="center">
  Made with ❤️, cutting chai ☕, and unadulterated bro vibes. <br>
  <b>Star this repo if you believe in bh-AI supremacy! ⭐</b>
</p>
