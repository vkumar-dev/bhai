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

## 🛠️ How to Implement `bhai` in 60 Seconds

Copy-paste the prompt below into your AI coding agent / IDE:

<details>
<summary>📋 <b>Click to copy the AI Agent Prompt to build `bhai`</b></summary>

```markdown
Hey Agent! Please build and install a lightweight CLI tool named `bhai` on my machine.

### Requirements:
1. **Language:** Use whatever is fastest and easiest for my system (e.g. Go, Rust, Python, or Node.js).
2. **Provider:** Connect it to my available AI provider or API key (e.g. Gemini, OpenAI, Claude, Groq, Ollama, or OpenRouter via env var).
3. **Behavior:**
   - When I type `bhai <query>`, pass everything after `bhai` as a natural language prompt to the LLM.
   - Persona: A supportive, witty, street-smart "Bhai / Bro" who is technically brilliant, helpful, humorous, and ends with brotherly assurance ("Bhai sambhal lega").
   - If the user asks for terminal actions (like fixing bugs, running scripts, reading files, searching logs), let `bhai` have tool-execution capability (or output the exact command and offer to run it).
4. **Hinglish & Multi-language Support:** Automatically detect if the user speaks Hinglish, Hindi, English, Spanish, etc., and respond in the same vibe.
5. **Install:** Ensure the binary/script is aliased or symlinked to my PATH as `bhai` so I can immediately run `bhai 2 aur 2 kitne hote hain`.
```

</details>

---

## 🎭 Persona Personalities (Configurable in your Bhai)

When generating your `bhai`, you can instruct it to adopt different modes:

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
