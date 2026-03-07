<!-- Custom animated header — no external dependencies -->
<img src="assets/header.svg" width="100%" alt="Zach Abraham — AI Infrastructure, Multi-Agent Systems, Automation"/>

<p align="center">
  <a href="https://zach-abraham.github.io/clawd-hq"><img src="https://img.shields.io/badge/Portfolio-zach--abraham.github.io-58a6ff?style=flat-square&logo=github-pages&logoColor=white"/></a>
  <a href="https://linkedin.com/in/zachabraham1"><img src="https://img.shields.io/badge/LinkedIn-zachabraham1-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:zrabraham@gmail.com"><img src="https://img.shields.io/badge/Email-zrabraham-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>
</p>

---

<!-- Bento grid: 2-column layout -->
<table>
<tr>
<td width="55%" valign="top">

### What I Build

I build **multi-agent AI systems** that run themselves. Eight specialized agents coordinate through a shared event bus and persistent memory layer — handling everything from prediction markets to job applications to infrastructure monitoring.

**The system is live.** Right now, on a Mac Mini in Houston, agents are trading Kalshi contracts, applying to jobs, monitoring five machines, and synthesizing cross-domain insights every six hours.

> *Automate the boring. Synthesize the complex. Sleep through the night.*

</td>
<td width="45%" valign="top">

### System at a Glance

```
┌─────────────────────────────┐
│ 🔴 HAL Orchestrator         │
├─────────────────────────────┤
│ 8 autonomous agents         │
│ 5-machine Tailscale mesh    │
│ SQLite event bus (pub/sub)  │
│ Mem0 persistent memory      │
│ 6-hour synthesis heartbeat  │
│ Telegram alert pipeline     │
│ A2A cross-machine protocol  │
└─────────────────────────────┘
```

</td>
</tr>
</table>

---

### Clawd HQ — Multi-Agent Orchestration Platform

<table>
<tr>
<td>

[![Architecture](https://img.shields.io/badge/Architecture_Docs-181717?style=flat-square&logo=github)](https://github.com/zach-abraham/clawd-hq)
[![Live Site](https://img.shields.io/badge/Portfolio-58a6ff?style=flat-square&logo=github-pages&logoColor=white)](https://zach-abraham.github.io/clawd-hq)

8 AI agents on a Mac Mini. Each has its own domain, memory scope, Telegram topic, and schedule. They coordinate through a SQLite event bus and Mem0-powered memory layer.

| Agent | Domain | Schedule |
|-------|--------|----------|
| **HAL** | Orchestration | Always-on |
| **Trader** | Prediction Markets | Every 4h |
| **Recruiter** | Job Automation | Every 4h |
| **Banker** | Personal Finance | Daily |
| **Professor** | Education | On-demand |
| **CEO** | Strategy | On-demand |
| **Sentinel** | Infrastructure | Hourly |
| **Trainer** | Fitness | On-demand |

</td>
</tr>
</table>

<details>
<summary><b>Architecture Deep Dive</b></summary>
<br/>

<table>
<tr>
<td width="50%">

**Cross-Agent Event Bus**

SQLite-backed pub/sub with WAL mode. Event categories: `decision`, `alert`, `state_change`, `discovery`. Severity escalation routes critical events to Telegram. HAL consumes all events during synthesis.

</td>
<td width="50%">

**HAL Synthesis Heartbeat**

Every 6 hours, HAL queries all agent memories and events, passes them through Gemini Flash for cross-domain pattern detection, then posts insights to Telegram and stores them in persistent memory.

</td>
</tr>
<tr>
<td width="50%">

**Dual-Namespace Memory**

Mem0 Cloud with two namespaces: personal (cross-device agent memory) and shared (multi-user collaboration). DLP sanitization layer strips secrets before storage.

</td>
<td width="50%">

**Infrastructure Mesh**

5-machine Tailscale mesh. LaunchAgent-based scheduling. Docker services (Uptime Kuma, Langfuse, Beszel, n8n). A2A protocol for cross-machine agent communication.

</td>
</tr>
</table>

</details>

---

### Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,bash,docker,linux,sqlite,git,github,githubactions&theme=dark&perline=8"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude-191919?style=flat-square&logo=anthropic&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white"/>
  <img src="https://img.shields.io/badge/Mem0-7C3AED?style=flat-square"/>
  <img src="https://img.shields.io/badge/Tailscale-000000?style=flat-square&logo=tailscale&logoColor=white"/>
  <img src="https://img.shields.io/badge/Telegram_Bot-26A5E4?style=flat-square&logo=telegram&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kalshi-000000?style=flat-square"/>
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white"/>
  <img src="https://img.shields.io/badge/LaunchAgents-000000?style=flat-square&logo=apple&logoColor=white"/>
</p>

---

<details>
<summary><b>GitHub Stats</b></summary>
<br/>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=zach-abraham&show_icons=true&theme=transparent&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=58A6FF&text_color=C9D1D9&count_private=true&ring_color=58A6FF" alt="GitHub Stats" height="165"/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=zach-abraham&theme=transparent&hide_border=true&background=0D1117&stroke=30363d&ring=58A6FF&fire=f78166&currStreakLabel=58A6FF&sideLabels=8b949e&dates=8b949e&currStreakNum=c9d1d9&sideNums=c9d1d9" alt="GitHub Streak" height="165"/>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=zach-abraham&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=58A6FF&line=58A6FF&point=c9d1d9&area=true&area_color=58A6FF" alt="Activity Graph" width="100%"/>
</p>

</details>

---

<p align="center">
  <sub>Houston, TX · Built with Claude, Gemini, and way too much caffeine</sub>
</p>
