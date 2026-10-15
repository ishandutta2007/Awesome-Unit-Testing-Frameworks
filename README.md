# Awesome-Unit-Testing-Frameworks

## Top Uptime Monitoring Tools Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Endpoint Probing, Status Pages & Incident Notification*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Uptime Monitoring**. These tools probe websites, APIs, ports, and infrastructure on scheduled intervals, alert when something breaks, and publish status pages so customers and internal teams know what's happening.

**Examples** include UptimeRobot, Pingdom, StatusCake, Better Uptime, Site24x7, Datadog Synthetics, Freshping, Uptrends, Cronitor, and Checkly (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom monitor types, and transparent alerting — ideal for teams prioritizing data sovereignty, developers building observability pipelines, and organizations avoiding per-monitor SaaS pricing.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[UptimeRobot](https://uptimerobot.com/)**  
  The reference point for uptime monitoring SaaS. Free tier: 50 monitors, 5-minute intervals. Solo: $84/year for 10 monitors, 60-second intervals. Global probe locations require paid tiers [citation:3].

- **[Pingdom](https://www.pingdom.com/)**  
  Long-standing synthetic monitoring and uptime service with real browser checks and transaction monitoring.

- **[StatusCake](https://www.statuscake.com/)**  
  Uptime, page speed, SSL, and domain monitoring with free tier and paid scaling.

- **[Better Uptime](https://betteruptime.com/)**  
  Uptime monitoring with on-call scheduling, incident management, and status pages.

- **[Site24x7](https://www.site24x7.com/)**  
  Full-stack monitoring including uptime, APM, server, and network monitoring.

- **[Datadog Synthetics](https://www.datadoghq.com/)**  
  Synthetic monitoring integrated with Datadog's observability platform.

- **[Freshping](https://www.freshworks.com/)**  
  Free uptime monitoring from Freshworks with 50 monitors and 1-minute intervals.

- **[Uptrends](https://www.uptrends.com/)**  
  Synthetic monitoring with multi-step transactions and global probe locations.

- **[Cronitor](https://cronitor.io/)**  
  Cron job and background task monitoring with uptime checks.

- **[Checkly](https://www.checklyhq.com/)**  
  Synthetic monitoring with Playwright-based browser checks and API monitoring.

## Open-Source GitHub Projects

- **[Uptime Kuma](https://github.com/louislam/uptime-kuma)**  
  **The most widely adopted self-hosted uptime monitoring tool** — 89,900+ GitHub stars, MIT licensed, actively maintained [citation:4][citation:6]. "A fancy self-hosted monitoring tool like Uptime Robot." Features HTTP(s), TCP, Ping, DNS, Push, Docker, gRPC, and Steam monitors with 90+ notification integrations. Beautiful responsive UI with status pages and multi-language support. The default recommendation for anyone self-hosting uptime monitoring [citation:4].

- **[Peekaping](https://github.com/0xfurai/peekaping)**  
  **API-first Uptime Kuma alternative built in Go** with strict typing and extensible architecture [citation:1]. Supports HTTP, TCP, Ping, DNS, Push, Docker, gRPC, SNMP, PostgreSQL, MSSQL, MongoDB, Redis, MySQL, MQTT, RabbitMQ, and Kafka monitors. 22+ alert channels including Telegram, Slack, Discord, PagerDuty, and Gotify. Status pages with SVG badges, MFA, brute-force protection, and SSL expiry checks. Docker + SQLite/PostgreSQL/MongoDB [citation:1].

- **[Asura](https://github.com/y0f/Asura)**  
  **Single-binary Uptime Kuma alternative** with 19 monitor types and 13 notification channels [citation:8]. Runs on ~20MB RAM with SQLite built in. Features multi-step HTTP chains, anomaly detection with statistical baselines, distributed probe agents, public status pages with 90-day uptime bars, incident severity levels, escalation policies, SLA tracking, and AES-256-GCM encryption at rest. Scales to 1000+ monitors on a $5 VPS [citation:8].

- **[Kuvasz](https://github.com/kuvasz-uptime/kuvasz)**  
  **Performant uptime and SSL monitoring service** built in Kotlin [citation:3][citation:9]. Features HTTP(s), SSL cert, heartbeat/push, Ping, TCP, and DNS monitoring with record-change detection. Per-monitor notification channels, public/private status pages, REST API, OpenTelemetry and Prometheus exporters, Home Assistant integration, MCP server for AI assistants, and maintenance windows [citation:3].

- **[Gatus](https://github.com/TwiN/gatus)**  
  **Automated service health dashboard** with 7,400+ GitHub stars, Apache 2.0 licensed [citation:5][citation:12]. Go-based, config-driven with YAML. Supports HTTP, TCP, ICMP, and DNS checks with assertions, conditions, and alerting to Slack, PagerDuty, and more. Designed for developers who want health checks defined as code [citation:6].

- **[Checkmate](https://github.com/bluewave-labs/checkmate)**  
  **Open-source infrastructure monitoring** with uptime, page speed (Lighthouse), and server hardware monitoring (CPU, memory, disk, network) [citation:10]. Monitors HTTP, HTTPS, Ping, Docker, Port, Game, gRPC, and WebSocket. Status pages with incident tracking. Notifications to Slack, Discord, Webhook, PagerDuty, and Matrix. Docker + Nginx Proxy Manager deployment [citation:10].

- **[Upright](https://github.com/basecamp/upright)**  
  **37signals' open-source synthetic monitoring system** for Basecamp, HEY, and Fizzy [citation:7]. Rails engine deployed to cheap VPS nodes via Kamal. **Playwright probes** run real browser checks with video recording on failure. Also supports HTTP, SMTP, and Traceroute (MTR) probes. Multi-site data distinguishes regional blips from real outages. Prometheus metrics + AlertManager notifications. Runs across 5 global sites for ~$110/month [citation:7].

- **[OpenStatus](https://github.com/openstatusHQ/openstatus)**  
  **Open-source synthetic monitoring and status page platform** built with Next.js and Tailwind [citation:14]. Global monitoring from multiple locations, monitoring-as-code with YAML, CI/CD integration, and customizable public/private status pages. Docker-based self-hosting [citation:14].

- **[OneUptime](https://github.com/OneUptime/oneuptime)**  
  **Complete open-source observability platform** replacing Pingdom, StatusPage.io, PagerDuty, Incident.io, Datadog, Loggly, and Sentry in one Apache 2.0 self-hosted app [citation:17]. Uptime monitoring, status pages, on-call scheduling, incident management, APM, logs, metrics, error tracking, and AI-powered auto-fix PR generation. Docker Compose for homelabs, Helm for production [citation:17].

### Additional Strong Open-Source Options

- **cState** — Static status page for Hugo. Clean, minimal JS, optional admin panel. MIT licensed [citation:6].
- **Kener** — Status page with incident management, easy to customize. Node.js/Docker [citation:6].
- **StatPing.ng** — Easy-to-use status page for websites and applications. GPL-3.0 [citation:6].
- **Upptime** — Uptime monitor powered entirely by GitHub Actions and Issues. Zero infrastructure [citation:9].
- **MOSSBoard** — Vue 3 status board with admin interface, incident tracking, and fullscreen monitor view. GPL-3.0 [citation:13].

**Frameworks for building custom systems**: Combine **Uptime Kuma** or **Peekaping** for general-purpose uptime monitoring, **Asura** for single-binary low-resource deployments, **Gatus** for config-as-code health checks, **Upright** for Playwright-based browser flow testing, and **OneUptime** for a complete observability stack replacing multiple SaaS tools [citation:17].

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Uptime monitoring tools must comply with applicable regulations and should not be used to monitor systems you do not own or have permission to probe. **False positives and false negatives are inherent in any monitoring system** — multi-site probing and alert correlation reduce but do not eliminate noise [citation:7]. Production alerting should be tuned to avoid fatigue.
- Self-hosted open-source solutions require proper security hardening, notification credential management, and monitoring of the monitor itself.

---

**Made for SREs, DevOps engineers, platform teams, and developers building reliable infrastructure.**  
Let's make uptime monitoring more open, self-hostable, and developer-friendly.
