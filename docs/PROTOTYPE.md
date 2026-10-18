# Divisional Rollup — interactive UX prototype

Open the [GitHub Pages prototype](https://carlobarone-info.github.io/gstht/) once Pages is enabled for `main` → `/docs`.

## What this is

A low-fidelity frontend exploration that demonstrates a factual divisional rollup and navigation from division → team → pipeline. It uses fictional data only; no backend, authentication, live monitoring, severity scoring, or operational integrations.

The example has 5,000 pipelines: 4,700 succeeded, 100 failed and 200 not run yet, across eight teams. Team cards are sorted by failure rate, not business importance. Pipeline details are illustrative samples rather than exhaustive inventories.

## Why this approach

- Communicate known execution states rather than asserting an unsupported overall health grade.
- Surface failures without equating failure counts or rates with severity.
- Use ownership to group information and enable drill-down.
- Give dependent engineers enough context to follow up without inventing a messaging system.

## Publishing

Repository **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `/docs` → Save**.

**Privacy warning:** GitHub Free requires a public repository for Pages. GitHub Pro and eligible organization plans allow Pages from private repositories, but the published website is still generally public. Do not change this repository to private before checking your plan and Pages behaviour.
