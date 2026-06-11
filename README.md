<!-- Custom animated header — no external dependencies -->
<img src="assets/header.svg" width="100%" alt="Zach Abraham — AI Infrastructure, Multi-Agent Systems, Automation"/>

<p align="center">
  <a href="https://linkedin.com/in/zacharyrabraham"><img src="https://img.shields.io/badge/LinkedIn-zacharyrabraham-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:zrabraham@gmail.com"><img src="https://img.shields.io/badge/Email-zrabraham-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>
  <img src="https://img.shields.io/badge/Houston,%20TX-open%20to%20remote-lightgrey?style=flat-square"/>
</p>

---

<table>
<tr>
<td width="55%" valign="top">

### What I Build

I build **multi-agent AI systems that run themselves** — fleets of specialized agents that coordinate through a shared event bus and a persistent memory layer, with multi-provider LLM routing, self-healing automation, and cross-agent (A2A) communication.

**It's real infrastructure, not slideware.** Most of it runs 24/7 on a home server cluster: LLM routing with automatic failover, scheduled agents, health monitoring, and an evaluator loop that catches failures and repairs or escalates them without a human in the loop.

By day I'm an **IT systems & endpoint engineer** (Intune/MECM, M365, PowerShell/Python automation, multi-site server migrations). The systems below are where I push that further.

> *Automate the boring. Make it self-healing. Sleep through the night.*

</td>
<td width="45%" valign="top">

### System at a Glance

```
┌─────────────────────────────┐
│ HAL Orchestrator            │
├─────────────────────────────┤
│ Fleet of scoped agents      │
│ Event bus (pub/sub, WAL)    │
│ Persistent memory layer     │
│ 6-provider LLM failover     │
│ Self-healing scheduler      │
│ A2A cross-agent protocol    │
│ Telegram / CLI interface    │
└─────────────────────────────┘
```

</td>
</tr>
</table>

---

### Selected Work

[![clawd-multi-agent](https://img.shields.io/badge/clawd--multi--agent-181717?style=flat-square&logo=github)](https://github.com/zach-abraham/clawd-multi-agent)

A multi-agent system with domain-scoped agents, event-driven coordination, and a self-improving infrastructure layer. More flagship repos (multi-provider LLM orchestrator, A2A protocol server, persistent-memory stack) are being extracted from the live systems and published — clean, runnable, and secret-free.

<details>
<summary><b>Architecture Deep Dive</b></summary>
<br/>

<table>
<tr>
<td width="50%">

**Cross-Agent Event Bus**

SQLite-backed pub/sub with WAL mode. Event categories: `decision`, `alert`, `state_change`, `discovery`. Severity escalation routes critical events to a notification pipeline. The orchestrator consumes all events during synthesis.

</td>
<td width="50%">

**Synthesis Heartbeat**

On a schedule, the orchestrator queries every agent's memory and recent events, runs them through an LLM for cross-domain pattern detection, then surfaces insights and stores them in persistent memory.

</td>
</tr>
<tr>
<td width="50%">

**Multi-Provider LLM Routing**

Automatic failover and cost-aware fallback across six providers (Cerebras → Groq → NVIDIA NIM → SambaNova → local Ollama → Gemini), so a single rate-limit or outage never takes the system down.

</td>
<td width="50%">

**Persistent Memory + A2A**

A durable memory stack (PostgreSQL + Redis + Neo4j knowledge graph) gives agents long-term recall instead of stateless prompts. An Agent-to-Agent protocol server lets independent agents discover and delegate across machines.

</td>
</tr>
</table>

</details>

---

### Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,bash,docker,linux,postgres,redis,sqlite,git,github,githubactions&theme=dark&perline=10"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude-191919?style=flat-square&logo=anthropic&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white"/>
  <img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white"/>
  <img src="https://img.shields.io/badge/MCP-7C3AED?style=flat-square"/>
  <img src="https://img.shields.io/badge/A2A_Protocol-1F6FEB?style=flat-square"/>
  <img src="https://img.shields.io/badge/Neo4j-008CC1?style=flat-square&logo=neo4j&logoColor=white"/>
  <img src="https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white"/>
  <img src="https://img.shields.io/badge/Intune%20%2F%20M365-0078D4?style=flat-square&logo=microsoft&logoColor=white"/>
</p>

<p align="center">
  <sub>Open to <b>Systems / Infrastructure / Endpoint / Automation</b> engineering roles where IT ops meets real software.</sub>
</p>

---

<picture>
  <img src="assets/snake-dark.svg" alt="Snake contribution graph" width="100%"/>
</picture>

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
  <sub>Houston, TX · AI infrastructure, multi-agent systems, automation</sub>
</p>
