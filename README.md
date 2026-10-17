# gstht

A small starter for exploring a division-level data-health interface.

> Work in progress. All pipeline data in this repository is fictional.

## Run locally

Requires Node.js 20+.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite. Run `npm run build` to check the production build.

## Structure

- `src/App.tsx` — basic division → team → pipeline navigation.
- `src/data.ts` — editable mock data and state types.
- `src/styles.css` — responsive starter styles.
- `docs/presentation-outline.md` — slide outline and research prompts.

## Intent

This is a **design exploration scaffold**, not a production monitoring system. It has no backend, ingestion, authentication, incident management, or alerting. The rollup rule is a starting hypothesis to examine, not a final decision.

## Next steps

1. Audit the three reference approaches and write down what to keep/discard.
2. Define the classification and divisional rollup rule, including edge cases.
3. Iterate on the division → team → pipeline drill-down.
4. Capture decisions and trade-offs in the presentation outline.

Keep the final deliverable focused on rationale and design rather than implementation detail.
