---
name: dax
version: 0.21.0
description: Write, debug, and optimize DAX in semantic models. Automatically invoke when the user asks to "write DAX", "optimize DAX", "fix slow DAX", "DAX performance", "tune a measure", "debug a measure", "DAX anti-patterns", or mentions slow queries, server timings, or DAX authoring.
---

# DAX

Skills and references for writing, debugging, and optimizing DAX in semantic models.

## Optimization

For systematic DAX query performance optimization, read the full reference before starting:

**[DAX Performance Optimization Guide](./references/dax-performance-optimization.md)** — Tiered framework (4 tiers from safe DAX rewrites to model/layout changes), phased workflow, engine internals (FE/SE, xmSQL, fusion), trace diagnostics, and a pattern catalog of 27+ named patterns (DAX001–DL002).

The guide covers:
- **Tier 1** — DAX pattern rewrites (auto-apply, semantic equivalence required)
- **Tier 2** — Query structure changes (user approval required)
- **Tier 3** — Model changes (high caution)
- **Tier 4** — Direct Lake layout (ETL/pipeline scope)

For trace capture, the approach depends on available tooling. See the [`connect-pbid` skill](../../pbi-desktop/skills/connect-pbid/) for PowerShell-based performance profiling, or use DAX Studio / Fabric Workspace Monitoring.

## References

- **[`references/dax-performance-optimization.md`](./references/dax-performance-optimization.md)** — Complete optimization framework and pattern catalog

## Related Skills

- [`review-semantic-model`](../review-semantic-model/) — Model auditing including DAX anti-patterns and best practices
- [`connect-pbid` (pbi-desktop plugin)](../../pbi-desktop/skills/connect-pbid/) — Trace capture, performance profiling, EVALUATEANDLOG debugging
- [`lineage-analysis`](../lineage-analysis/) — Impact analysis before model changes
