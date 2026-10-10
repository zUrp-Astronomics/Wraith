# Wraith

All-in-one mount controller on a Raspberry Pi Compute Module 5 — in design phase: no code, no
hardware files, no test suite yet. What the product is meant to do is described only in `README.md`
and `9_Assets/zurp.yml`.

## Stack

Planned hardware, as written in `README.md` and `9_Assets/zurp.yml`: a Raspberry Pi Compute Module 5
running mount control, the imaging pipeline, the astrometry solver and a web UI on one board. No
software language or framework is chosen in the repository yet — do not pick one unless a brief
says so.

## Conventions

- `README.md`, `9_Assets/`, `LICENSE`, `LICENSE-HARDWARE` and `.github/workflows/zurp-site.yml` are the
  showcase, written by the zUrp-Astronomics organisation for all its products at once: a project
  ticket does not touch them.
- The `0_` to `9_` folder tree and the naming of board files are defined by the organisation in the
  section "Arborescence et nommage des dépôts produit" of its README kit:
  https://github.com/zUrp-Astronomics/.github/blob/main/readme-kit/README.md — follow it, do not
  restate it here.

## Gotchas

- CI (`.gitea/workflows/ci.yml`) runs only the green placeholder job `no-harness-yet`: a green CI
  proves nothing about the code. The ticket that brings the first test suite replaces that step with
  the real command and adds `## Test` (the identical command) and `## Harness` (the suite's paths)
  to this file.
