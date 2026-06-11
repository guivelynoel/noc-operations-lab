# NOC Operations Lab

A hands-on portfolio demonstrating core **Network Operations Center (L1)** skills: 24x7-style infrastructure monitoring, incident detection and triage, ITIL-aligned incident management, and health-check automation.

**Author:** Guively Noel — Atlanta, GA
[guivelynoel.com](https://guivelynoel.com) · [LinkedIn](https://www.linkedin.com/in/guivelynoel) · nguively@gmail.com
*CCNA · CompTIA Security+ · CompTIA CySA+ · Azure Fundamentals*

---

## Why this lab exists

L1 NOC work is a cycle: **monitor → detect → triage → escalate or resolve → document.**
Each project in this repository implements one part of that cycle with real tools, real alerts, and real documentation — not theory.

```
 ┌─────────────┐     ┌──────────────┐     ┌──────────────────┐
 │  MONITORING  │ ──▶ │   INCIDENT    │ ──▶ │   AUTOMATION /    │
 │  Lab 01      │     │   WORKFLOW    │     │   HEALTH CHECKS   │
 │  Zabbix      │     │   Lab 02      │     │   Lab 03          │
 │  alerts fire │     │  Jira + SOPs  │     │  Bash/PowerShell  │
 └─────────────┘     └──────────────┘     └──────────────────┘
```

## Projects

| # | Project | Tools | NOC skills demonstrated |
|---|---------|-------|------------------------|
| 01 | [24x7 Monitoring Lab](./01-zabbix-monitoring/) | Zabbix 7.0, Docker Compose, PostgreSQL, Nginx | Server/application monitoring, trigger configuration, alerting, outage simulation |
| 02 | [Incident Management Workflow](./02-incident-workflow/) | Jira, ITIL v4 practices | Incident lifecycle, SLA-based escalation, L1 runbooks/SOPs |
| 03 | [Health-Check Automation](./03-health-check-scripts/) | Bash, PowerShell, cron | Routine health checks, log generation, failure alerting |

## Skills map (to a typical L1 NOC job description)

| Job requirement | Where it's demonstrated |
|---|---|
| Monitor infrastructure, servers, applications with monitoring tools | Lab 01 — Zabbix dashboards, agents, web-scenario checks |
| Identify, log, and respond to alerts and incidents | Lab 01 — simulated outage, alert fired and acknowledged |
| Initial troubleshooting and root cause identification | Lab 02 — runbooks with step-by-step L1 diagnostics |
| Escalate to L2/L3 per SLA | Lab 02 — escalation matrix with SLA timers |
| Maintain tickets and documentation in ITSM tools | Lab 02 — Jira incident workflow with worked examples |
| Routine health checks of systems and network devices | Lab 03 — scheduled scripts with timestamped logs |
| Scripting (Bash, PowerShell) | Lab 03 — both implementations, same checks |

## Environment

All labs run locally on macOS using Docker Desktop — no paid services required. Every project includes its own README with architecture, deployment steps, and screenshots of the working system.

---

*This repository is actively maintained as I continue building NOC and infrastructure skills.*
