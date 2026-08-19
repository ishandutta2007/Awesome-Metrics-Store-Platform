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
- **[Transform](https://transform.co/)**  
  Metrics store platform (acquired/influenced by the broader dbt ecosystem) focused on governed, reusable business metrics.

- **[Cube Cloud](https://cube.dev/)**  
  Managed service of the open-source Cube semantic layer, providing caching, APIs, and embedded analytics on top of a headless metrics store.

- **[dbt Semantic Layer](https://www.getdbt.com/)**  
  Cloud-hosted semantic layer powered by MetricFlow that lets teams define metrics inside dbt projects and query them consistently across tools.

- **[Omni](https://omni.co/)**  
  Modern analytics platform with strong semantic modeling and self-serve exploration capabilities.

- **[MetricFlow (via dbt)](https://docs.getdbt.com/)**  
  The query engine and metric definition framework that powers the dbt Semantic Layer (also available as open source).

- **[Lightdash Cloud](https://www.lightdash.com/)**  
  Managed offering of the open-source Lightdash platform, providing governed BI and metrics exploration on top of dbt projects.

- **[GoodData](https://www.gooddata.com/)**  
  Analytics and semantic-layer platform focused on governed metrics, embedding, and multi-tenant analytics.

- **[Looker (Google Cloud)](https://cloud.google.com/looker)**  
  Established BI platform with LookML as its powerful semantic modeling language and governed metrics layer.

- **[Hex](https://hex.tech/)**  
  Collaborative data workspace that integrates with semantic layers and supports governed metric consumption alongside notebooks and apps.

- **[AtScale](https://www.atscale.com/)**  
  Enterprise semantic layer and virtual OLAP platform that provides consistent metrics and high-performance query acceleration across BI tools.

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