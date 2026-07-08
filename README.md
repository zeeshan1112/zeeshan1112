<h1 align="center">⚡ ZEESHAN AHMAD</h1>
<p align="center">
  <b>Principal Software Engineer & AI Architect</b><br>
  Specializing in Stateful Multi-Agent Systems, Secure Runtimes, and B2B SaaS Infrastructure.
</p>

<p align="center">
  <a href="https://linkedin.com/in/zeeshanahmad2/"><img src="https://img.shields.io/badge/LinkedIn-Zeeshan--Ahmad-blue?style=for-the-badge&logo=linkedin&logoColor=white&color=0284c7" alt="LinkedIn" /></a>
  <a href="mailto:zeeshan.ahmad.career@gmail.com"><img src="https://img.shields.io/badge/Email-Zeeshan--Ahmad-blue?style=for-the-badge&logo=gmail&logoColor=white&color=ea4335" alt="Email" /></a>
  <a href="https://zeeshanahmad.dev"><img src="https://img.shields.io/badge/Portfolio-zeeshanahmad.dev-blue?style=for-the-badge&logo=googlechrome&logoColor=white&color=0f172a" alt="Website" /></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-PMTS%20%40%20Oracle-3b82f6?style=flat-square&logo=oracle&logoColor=white" alt="Oracle PMTS" />
  <img src="https://img.shields.io/badge/MS%20CS-AI%20Specialization-f59e0b?style=flat-square&logo=georgiainstituteoftechnology&logoColor=white" alt="Georgia Tech AI" />
  <img src="https://img.shields.io/badge/GPA-4.0%20%2F%204.0-10b981?style=flat-square" alt="GPA" />
  <img src="https://komarev.com/ghpvc/?username=zeeshan1112&color=3b82f6&style=flat-square" alt="Profile Views" />
</p>

---

### 🧬 Professional Overview

I am an engineering leader with **10+ years of experience** building high-performance enterprise applications, now designing and building stateful multi-agent workflows, MCP-powered agent runtimes, LLM evaluation pipelines, and context-optimization layers.

---

### 📐 Featured System Architecture: Stateful Agent Platform

To solve the challenges of context window degradation, runtime tool safety, and non-deterministic LLM output, this architecture incorporates stateful orchestration, sandboxed execution, and human-in-the-loop validation:

```mermaid
flowchart TD
    %% Define Styles
    classDef client fill:#1e293b,stroke:#38bdf8,stroke-width:2px,color:#f8fafc;
    classDef agent fill:#0f172a,stroke:#3b82f6,stroke-width:2px,color:#f8fafc;
    classDef engine fill:#1e1b4b,stroke:#818cf8,stroke-width:2px,color:#f8fafc;
    classDef db fill:#022c22,stroke:#34d399,stroke-width:2px,color:#f8fafc;
    classDef guard fill:#450a0a,stroke:#f87171,stroke-width:2px,color:#f8fafc;

    %% Nodes
    User(["User (Natural Language)"])
    UI["Analytics Interface / Client"]
    Router{"Orchestrator Router"}
    
    subgraph AgenticCore [Agentic Platform Runtime]
        Planner["Planning Agent (ToT / ReAct)"]
        ExecutionDB[("State Store (Graph Memory)")]
        MCPRuntime["MCP Tool Execution Runtime"]
    end
    
    subgraph Guardrails [Safety & Validation]
        PromptGuard["Input Guardrail (Injection Check)"]
        HITL{"HITL Checkpoint"}
        ExecGuard["Execution Guardrail (Rule Engine)"]
    end

    TargetAPI[("Enterprise Semantic Model / Database")]

    %% Connections
    User -->|Prompts| UI
    UI --> PromptGuard
    PromptGuard -->|Clean Request| Router
    Router -->|State & Context| Planner
    Planner -->|Action DAG| ExecutionDB
    ExecutionDB -->|Proposed Tool Call| HITL
    
    HITL -->|Approved| ExecGuard
    HITL -->|Rejected| Planner
    
    ExecGuard -->|Valid Call| MCPRuntime
    MCPRuntime -->|Execute| TargetAPI
    TargetAPI -->|Results| ExecutionDB
    ExecutionDB -->|Next Step / Final Output| Router
    Router -->|Response| UI

    %% Apply Styles
    class User,UI client;
    class Router,Planner,MCPRuntime agent;
    class ExecutionDB db;
    class PromptGuard,ExecGuard,HITL guard;
    class TargetAPI db;
```

---

### 🛠️ Technical Ecosystem
| category | tools & technologies |
| :--- | :--- |
| **AI / LLM** | LangGraph, Model Context Protocol (MCP), Prompt Engineering, LLM Evaluation (Benchmarking Harnesses), NLP |
| **Languages** | Python, TypeScript, Java, Node.js, JavaScript (ES6+), T-SQL |
| **Frameworks** | Next.js, React, Spring Boot, Supabase, Lucene, Express, Docker, Tailwind CSS |
| **Editors** | Cursor, Claude Code, GitHub Copilot, Antigravity Codex |

---

### 🌟 Featured Architecture

<table border="0" width="100%">
<tr>
<td width="50%" valign="top">
<h4>🌐 <a href="https://github.com/zeeshan1112/zerowebtools">ZeroWebTools</a></h4>
<p>Privacy-first browser utility suite of 55+ developer, PDF, and image tools running 100% client-side via WebAssembly. Engineered with a modular TypeScript core library shared across the web app and a Chrome Extension.</p>
<p>
  <img src="https://img.shields.io/badge/TypeScript-%233178C6.svg?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/WebAssembly-%23654FF0.svg?style=flat-square&logo=webassembly&logoColor=white" alt="WebAssembly" />
  <img src="https://img.shields.io/badge/Chrome_Extension-%234285F4.svg?style=flat-square&logo=google-chrome&logoColor=white" alt="Chrome Extension" />
</p>
</td>
<td width="50%" valign="top">
<h4>🏥 <a href="#">DocScale (Private)</a></h4>
<p>Healthcare B2B SaaS platform that automates clinic site provisioning in seconds. Architected with React/Vite dashboards, Next.js App Router for server-side rendering (SSR), and PostgreSQL Row Level Security (RLS) for tenant isolation.</p>
<p>
  <img src="https://img.shields.io/badge/Next.js-black?style=flat-square&logo=next.js&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/Supabase-3FC08D?style=flat-square&logo=supabase&logoColor=white" alt="Supabase" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
</p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<h4>🕰️ <a href="https://github.com/zeeshan1112/KeepMacAwake">KeepMacAwake</a></h4>
<p>Native macOS menu-bar utility preventing system sleep by posting synthetic user activity events directly into the CoreGraphics HID queue (bypassing macOS sleep policies without visible cursor movement).</p>
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/macOS_Quartz-000000?style=flat-square&logo=apple&logoColor=white" alt="Quartz API" />
  <img src="https://img.shields.io/badge/RumP5-grey?style=flat-square" alt="Rumps" />
</p>
</td>
<td width="50%" valign="top">
<h4>🖥️ <a href="https://github.com/zeeshanahmad-io/zeeshanahmad-dev-showcase">Zeeshan Ahmad Dev Showcase</a></h4>
<p>Professional developer portfolio and technical blog built using React/Vite and Keystatic CMS, featuring hybrid Markdown storage and reader mode layout configurations.</p>
<p>
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/TypeScript-%233178C6.svg?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Keystatic-grey?style=flat-square" alt="Keystatic" />
</p>
</td>
</tr>
</table>

---

### 📈 Global Impact & Metrics
<p align="center">
<img src="https://github-readme-stats-alpha.vercel.app/api?username=zeeshan1112&show_icons=true&theme=radical&rank_icon=github&count_private=true&include_all_commits=false" width="48%" />
<img src="https://github-readme-stats-alpha.vercel.app/api/top-langs/?username=zeeshan1112&layout=compact&theme=radical&hide=html,css" width="48%" />
</p>

<p align="center">
<img src="https://github-readme-streak-stats.herokuapp.com/?user=zeeshan1112&theme=radical&starting_year=2025" width="100%" />
</p>

---

<p align="center">
<i>"For you to do something new, you need to stop doing something old."</i>
</p>
