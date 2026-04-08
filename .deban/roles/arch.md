---
role: arch
owner: Gerald (Jelaludo)
status: active
---

## Decisions

- 2026-04-08: Zero-build architecture. Single `index.html` with inline JSX transpiled by Babel standalone. CDN: React 18, ReactDOM 18, Babel standalone. No bundler, no node_modules. [[dev]] [[devops]]
- 2026-04-08: Persistence layer: localStorage only. Export via client-side Blob downloads (JSON + CSV). No backend, no database. [[dev]]

## Dead Ends

## Lessons

## Open Questions

- Future tabs beyond sardine tracker — will single-file approach scale?

## Assumptions

- Babel standalone transpilation is fast enough for ~1000 lines of JSX
- GitHub Pages serves static HTML without issues

## Dependencies

- [[devops]] for hosting
- [[dev]] for implementation

## Session Log

- 2026-04-08: Defined zero-build static architecture for GitHub Pages deployment
