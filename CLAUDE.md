# CLAUDE.md — Competitive Analysis Project

## Project Purpose

This repository contains a multi-agent competitive analysis of AI coding assistant orchestration tools.
Gas Town (gt) is compared against: Cursor Composer, Windsurf Cascade, Devin, OpenHands, SWE-agent.

## Agent Work Guidelines

### Report Format

All reports MUST be written in **Markdown** format with:
- Clear heading hierarchy (H1 for title, H2 for sections, H3 for subsections)
- At least one **Mermaid diagram** per report (architecture, comparison, flow, or matrix)
- Data presented in **Markdown tables** where applicable
- Minimum **2000 words** per individual report, **4000 words** for the final synthesis

### Output Locations

| Bead Type | Output File |
|-----------|-------------|
| Product overview & architecture | `reports/01-product-architecture.md` |
| Feature matrix | `reports/02-feature-matrix.md` |
| Pricing & business model | `reports/03-pricing-business.md` |
| Community & developer sentiment | `reports/04-community-sentiment.md` |
| SWOT analysis | `reports/05-swot-analysis.md` |
| Final synthesis | `final/compete-report.md` |

### Research Methodology

- Use web search to gather current (2025-2026) information
- Cite sources with URLs where possible
- Distinguish between verified facts and inferences
- If information is unavailable, state "Not publicly available" rather than guessing

### Completion Protocol

This is a **report-only** project. Polecats:
1. Write the report file to the specified path
2. Commit the report: `git add <file> && git commit -m "docs: <report-name> (<bead-id>)"`
3. Persist key findings to the bead: `bd update <bead-id> --notes "Report complete. Key findings: ..."`
4. Finish with: `gt done --cleanup-status clean`

### Mermaid Diagram Standards

Use fenced code blocks with `mermaid` language tag. Preferred diagram types:
- `graph TD` for architecture comparisons
- `quadrantChart` for positioning maps
- `xychart-beta` for quantitative comparisons
- `pie` for market share or category breakdowns
