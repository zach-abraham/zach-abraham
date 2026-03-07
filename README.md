<!-- Header -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:1a1e2e&height=220&section=header&text=Zach%20Abraham&fontSize=52&fontColor=c9d1d9&animation=fadeIn&fontAlignY=38&desc=AI%20Infrastructure%20%7C%20Multi-Agent%20Systems%20%7C%20Automation&descSize=16&descColor=8b949e&descAlignY=58"/>

<p align="center">
  <a href="https://zach-abraham.github.io/clawd-hq"><img src="https://img.shields.io/badge/Portfolio-zach--abraham.github.io-58a6ff?style=for-the-badge&logo=github-pages&logoColor=white"/></a>
  <a href="https://linkedin.com/in/zachabraham1"><img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:zrabraham@gmail.com"><img src="https://img.shields.io/badge/-Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=500&size=20&pause=1000&color=58A6FF&center=true&vCenter=true&random=false&width=620&lines=8+AI+agents+running+autonomously+on+a+Mac+Mini;Cross-domain+synthesis+via+shared+event+bus;Every+agent+has+memory%2C+a+schedule%2C+and+a+mission;Build+it+once%2C+automate+it+forever" alt="Typing SVG" />
</p>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## What I Build

I build **multi-agent AI systems** that run themselves. Eight specialized agents coordinate through a shared event bus and persistent memory layer, handling everything from prediction markets to job applications to infrastructure monitoring -- all without human intervention.

**The system is live.** Right now, on a Mac Mini in Houston, agents are trading Kalshi contracts, applying to jobs, monitoring five machines, and synthesizing cross-domain insights every six hours.

**My philosophy:** *Automate the boring. Synthesize the complex. Sleep through the night.*

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## Clawd HQ -- The Flagship

<table>
<tr>
<td width="60%">

### Multi-Agent AI Orchestration Platform

[![Repo](https://img.shields.io/badge/Architecture_Docs-181717?style=for-the-badge&logo=github)](https://github.com/zach-abraham/clawd-hq)
[![Live Site](https://img.shields.io/badge/Portfolio_Site-58a6ff?style=for-the-badge&logo=github-pages&logoColor=white)](https://zach-abraham.github.io/clawd-hq)

8 autonomous AI agents on a Mac Mini. Each has its own domain, memory scope, Telegram topic, and schedule. They share a SQLite event bus and Mem0-powered memory layer.

**Agents:** HAL (orchestrator), Trader (Kalshi markets), Recruiter (job automation), Banker (personal finance), Professor (education), CEO (strategy), Sentinel (infrastructure), Trainer (fitness)

`Claude` `Gemini` `SQLite` `Mem0` `Tailscale` `Telegram` `LaunchAgents`

</td>
<td width="40%">

```
 ┌──────────────────────────┐
 │      Mac Mini (M2)       │
 │  ┌─────┐ ┌──────┐       │
 │  │ HAL │ │Trader│ ...x8  │
 │  └──┬──┘ └──┬───┘       │
 │     │       │            │
 │  ┌──┴───────┴──────────┐ │
 │  │   SQLite Event Bus  │ │
 │  └─────────┬───────────┘ │
 │  ┌─────────┴───────────┐ │
 │  │   Mem0 Memory Layer │ │
 │  └─────────────────────┘ │
 │                          │
 │  OpenClaw ─ Telegram ─ A2A│
 └──────────────────────────┘
```

</td>
</tr>
</table>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## Architecture Highlights

<table>
<tr>
<td width="50%">

### Cross-Agent Event Bus
SQLite-backed pub/sub with WAL mode. Categories: `decision`, `alert`, `state_change`, `discovery`. Agents publish events and subscribe to feeds. HAL consumes everything during synthesis.

</td>
<td width="50%">

### HAL Synthesis Heartbeat
Every 6 hours, HAL queries all agent memories and events, passes them through Gemini Flash for cross-domain pattern detection, then posts insights to Telegram and stores them in persistent memory.

</td>
</tr>
<tr>
<td width="50%">

### Dual-Namespace Memory
Mem0 Cloud with two namespaces: personal (cross-device agent memory) and shared (multi-user collaboration). DLP sanitization layer strips secrets before storage.

</td>
<td width="50%">

### Infrastructure Mesh
5-machine Tailscale mesh. LaunchAgent-based scheduling. Docker services (Uptime Kuma, Langfuse, Beszel, n8n). A2A protocol for agent-to-agent communication across machines.

</td>
</tr>
</table>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## Tech I Work With

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,bash,docker,linux,sqlite,git,github,githubactions,tailwindcss,html,css,js&theme=dark&perline=12"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude-191919?style=flat-square&logo=anthropic&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white"/>
  <img src="https://img.shields.io/badge/Mem0-000000?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iMTAiLz48L3N2Zz4=&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tailscale-000000?style=flat-square&logo=tailscale&logoColor=white"/>
  <img src="https://img.shields.io/badge/Telegram_Bot-26A5E4?style=flat-square&logo=telegram&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kalshi_API-000000?style=flat-square"/>
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white"/>
  <img src="https://img.shields.io/badge/LaunchAgents-000000?style=flat-square&logo=apple&logoColor=white"/>
</p>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=zach-abraham&show_icons=true&theme=transparent&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=58A6FF&text_color=C9D1D9&count_private=true&ring_color=58A6FF" alt="GitHub Stats" height="165"/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=zach-abraham&theme=transparent&hide_border=true&background=0D1117&stroke=30363d&ring=58A6FF&fire=f78166&currStreakLabel=58A6FF&sideLabels=8b949e&dates=8b949e&currStreakNum=c9d1d9&sideNums=c9d1d9" alt="GitHub Streak" height="165"/>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=zach-abraham&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=58A6FF&line=58A6FF&point=c9d1d9&area=true&area_color=58A6FF" alt="Activity Graph" width="100%"/>
</p>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=zach-abraham&theme=onestar&no-frame=true&no-bg=true&column=7&margin-w=5&margin-h=5" alt="Trophies"/>
</p>

---

<p align="center">
  <em>Houston, TX</em>
</p>

<!-- Footer -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:1a1e2e&height=100&section=footer"/>
