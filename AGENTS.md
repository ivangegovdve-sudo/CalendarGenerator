# AGENTS.md - CalendarGenerator Working Guide

This repository is the source snapshot for the standalone CalendarGenerator app. Treat it as a static product and as an upstream reference for any calendar work that later gets embedded into Forest HUB or another repo.

## Goal

- preserve a working printable calendar generator
- keep the app fully usable as a standalone static page
- use this repo as the clean reference point for upstream behavior, licensing, and assets

## Current Idea And Progress

- Product idea:
  a simple printable yearly calendar creator with holiday lookup, custom images, and month captions
- Current state:
  mature single-page static app
- Local role:
  mostly a reference/source repo rather than the primary place for new feature work
- Product maturity:
  working for its original purpose, but still in legacy form with jQuery and a flat file structure

## Initial Setup Requirements

- no package manager or backend is required
- serve it from any static server from the repo root
- recommended local command:
  `python -m http.server 8080`
- open:
  `http://127.0.0.1:8080/calendario.html`

## Environments

- local development:
  static server only
- staging:
  not currently defined
- production:
  historically suitable for static hosting only

## Dependencies

- browser runtime
- jQuery loaded from CDN in the upstream page
- public holiday API:
  `https://kayaposoft.com/enrico/json/v1.0/`
- local image assets in `pics/`
- Apache-2.0 license obligations from the upstream project

## Backend Need

- backend required now:
  no
- backend recommended later:
  only if the project gains user accounts, saved templates, uploads, sharing, or export jobs

## How Development Should Progress

1. Keep the standalone app working before making stylistic changes.
2. Preserve upstream notices and the Apache-2.0 license text.
3. If the app is adapted into another repo, mark local modifications clearly there.
4. Use this repo as the behavioral reference for month rendering, image defaults, and holiday behavior.
5. Avoid turning this repo into a second product if the real working version already lives elsewhere.

## Practical Roadmap

- Short term:
  keep it runnable and clearly documented
- Medium term:
  decide whether this repo stays a reference mirror or becomes a maintained fork
- Long term:
  either archive it as upstream-source-only or modernize it with plain JS and a cleaner structure while preserving print fidelity

## End Goal

The end goal is a trustworthy static reference implementation of the calendar generator, with clear licensing, honest setup instructions, and no ambiguity about whether this repo is the source snapshot or the active customized product.
