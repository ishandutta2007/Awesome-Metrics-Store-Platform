# Awesome-Metrics-Store-Platform

## Top Metrics Store Platforms Ecosystem
**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Semantic Layers, Governed Metrics, Consistent Business Logic, Headless BI, Metric APIs & Single Source of Truth for Analytics*
**Last updated: August 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Metrics Stores** (also called semantic layers or metrics layers). These systems centralize the definition of business metrics so that every dashboard, application, AI agent, and analyst queries the same trusted logic instead of recreating calculations in silos.

**Examples** include Transform, Cube, dbt Semantic Layer, Omni, MetricFlow, Lightdash, GoodData, Looker, Hex, and AtScale (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project. Several leading platforms (Cube, MetricFlow, Lightdash) offer strong open-source cores, making self-hosted, Git-versioned metrics layers practical for modern data teams.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing | Free Tier Limits |
| :--- | :--- | :--- | :--- |
| **[Transform](https://transform.co/)** | Original pioneer metrics store platform; acquired by dbt Labs and integrated into dbt Semantic Layer / MetricFlow. | Standalone product retired; accessible via dbt Cloud starting at $100/developer seat/month | N/A (Integrated into dbt Cloud; offers 14-day dbt Cloud trial or dbt Cloud Developer free tier with 1 seat & 3,000 models/mo) |
| **[Cube Cloud](https://cube.dev/)** | Managed service for the Cube semantic layer, providing caching, pre-aggregations, APIs (SQL/REST/GraphQL), and embedded analytics. | Consumption-based starting at ~$0.10 / Cube Consumption Unit (CCU) (no fixed monthly minimum) | Free forever plan: Up to 2 shared deployments for dev/testing (no credit card required) |
| **[dbt Semantic Layer](https://www.getdbt.com/)** | Cloud-hosted semantic layer powered by MetricFlow to define governed metrics in dbt and query across BI tools. | Starts at $100/developer seat/month (Starter tier; full semantic integrations on Enterprise tier) | 14-day free trial of Team/Enterprise features; Free Developer tier includes 1 seat & 3,000 models/mo (Semantic Layer requires paid tier) |
| **[Omni](https://omni.co/)** | Modern analytics and BI platform with a built-in semantic modeling layer and point-and-click data exploration. | Sales-led starting from ~$1,000/month for small team deployments (custom quote based on user seats and scope) | 14-day customized free evaluation trial (available upon sales request/demo) |
| **[MetricFlow (via dbt Cloud)](https://docs.getdbt.com/)** | Governed metric definition framework and SQL compilation engine powering the dbt Semantic Layer. | Included with dbt Cloud Starter at $100/developer seat/month (Enterprise custom for advanced features) | Core engine is 100% free open-source (Apache 2.0); Cloud Semantic Layer includes 14-day free trial on dbt Cloud |
| **[Lightdash Cloud](https://www.lightdash.com/)** | Managed BI and metrics exploration platform native to dbt projects with AI data analyst capabilities. | Cloud Starter starts at $800/month (unlimited users); Cloud Pro starts at $2,400/month | 21-day free trial (no credit card required; core platform is free self-hosted open-source) |
| **[GoodData](https://www.gooddata.com/)** | Composable data analytics and semantic layer platform tailored for governed metrics and multi-tenant embedded analytics. | Platform fee starting at ~$1,500/month based on workspaces and data scale (custom quote) | 30-day full-featured free trial (no credit card required) |
| **[Looker (Google Cloud)](https://cloud.google.com/looker)** | Enterprise BI platform featuring LookML as its centralized semantic modeling language and governed metrics store. | Custom enterprise annual contracts starting at ~$3,000–$5,000/month (~$36,000–$60,000/year for Standard Edition) | 30-day free proof-of-concept / evaluation trial via Google Cloud sales |
| **[Hex](https://hex.tech/)** | Collaborative workspace combining notebooks, SQL, metrics layer integrations, and interactive app builder. | Professional plan starts at $36/editor/month (Team plan at $75/editor/month; free viewer seats) | Free forever Community plan: 1 editor, up to 5 projects, small compute profiles (4GB RAM, 0.5 CPU), 100 AI actions/month |
| **[AtScale](https://www.atscale.com/)** | Universal semantic layer and virtual OLAP platform optimizing governed metrics across data warehouses and BI tools. | Object-based consumption model starting at ~$2,500/month based on Deployed Semantic Objects (DSOs) | Free Developer Community Edition for building/testing semantic models; 30-day guided enterprise free trial upon request |

## Open-Source GitHub Projects
- **[Cube (Cube Core)](https://github.com/cube-js/cube)**  
  Leading open-source semantic layer and headless BI platform with pre-aggregations, multi-API access (SQL, REST, GraphQL), and strong support for embedded analytics.

- **[MetricFlow](https://github.com/dbt-labs/metricflow)**  
  Open-source metric definition and SQL compilation engine (Apache 2.0) that powers the dbt Semantic Layer and enables governed, reusable metrics in code.

- **[Lightdash](https://github.com/lightdash/lightdash)**  
  Open-source agentic BI platform that reads dbt project metadata, exposes governed metrics and dimensions, and supports dashboards, AI agents, and Git-based workflows.

- **[dbt Core + Semantic modeling](https://github.com/dbt-labs/dbt-core)**  
  The foundational open-source transformation framework; when combined with MetricFlow it becomes a powerful metrics-as-code system.

- **[Apache Superset](https://github.com/apache/superset)**  
  Open-source BI platform frequently paired with semantic layers; supports custom metrics and can consume governed definitions from Cube or similar tools.

- **[Metabase](https://github.com/metabase/metabase)**  
  Popular open-source BI tool that can sit on top of a metrics store or define simpler metrics directly.

- **[Malloy and other emerging semantic languages](https://github.com/)**  
  Experimental and production open-source approaches to defining semantic models and metrics in a portable way.

- **[Custom metrics layers on DuckDB / Arrow](https://github.com/)**  
  Lightweight open-source projects that implement metric stores or semantic caching on modern analytical engines.

- **[Open Semantic Interchange (OSI) related work](https://github.com/)**  
  Community and vendor efforts aimed at portable metric and semantic model formats across tools.

- **[Headless BI examples and starters](https://github.com/)**  
  Reference implementations showing how to expose Cube or MetricFlow metrics to applications, AI agents, and BI tools.

### Additional Strong Open-Source Options
- Evidence, Rill, and other code-first or embedded analytics tools that benefit from an upstream metrics layer.
- SQLMesh and other transformation frameworks exploring semantic/metric capabilities.
- Open catalog and governance tools that document and version metric definitions.
- MCP / agent interfaces that expose governed metrics to AI coding and analysis agents.
- Pre-aggregation and caching patterns implemented with open technologies (Redis, DuckDB, etc.).

**Frameworks for building custom systems**: Define metrics in **MetricFlow** YAML (inside a dbt project) or in **Cube** data models, serve them via Cube’s APIs or the dbt Semantic Layer interfaces, and consume them from **Lightdash**, Superset, Metabase, notebooks, or custom applications. Version everything in Git, test metric changes in CI, and use pre-aggregations or warehouse materializations for performance. This stack gives a fully open, portable metrics store.

## How to Contribute
1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer
- This is a **community-curated** list — not exhaustive and not an endorsement.
- A metrics store is only as trustworthy as its definitions, tests, and ownership. Open-source tools provide excellent transparency and control but still require strong data governance, access controls, and documentation practices.
- Always validate critical business metrics against source systems and establish clear ownership before treating any layer as the single source of truth.

---
**Made for analytics engineers, data platform teams, and organizations that want consistent, governed metrics.**
Let's make the semantic layer open, portable, and owned by the teams who use it.