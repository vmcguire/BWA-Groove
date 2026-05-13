# BWA-Groove

Capture / extract groove (tap-along, audio file, manual swing). Writes to shared/groove/.

**Category B** · **Tier 5** · part of the
[Bandwidth Audio](https://github.com/vmcguire) plugin ecosystem.

---

## What this is

BWA-Groove captures or extracts the song's groove — the canonical timing the rest of the BWA ecosystem snaps TO instead of snapping the user away from. Three modes: tap-along (user plays along), audio extraction (analyze a reference), manual swing.

Result lands in shared/groove/, consumed by every Cat B plugin (Roll, Fill, Transition, Stutter, Form) and BWA-Click (which plays the captured groove as a click track). Inside a host DAW, Groove is host-synced; inside BWA Studio (post-funding), Groove IS the grid.

For the broader story of *what BWA is building and why*, see
[BWA-Architecture](https://github.com/vmcguire/BWA-Architecture) —
specifically:

- [`USER-STORY-MAP.md`](https://github.com/vmcguire/BWA-Architecture/blob/main/docs/USER-STORY-MAP.md)
  — where this plugin sits in the bedroom-producer journey (Stage 5 — ARRANGE).
- [`ECOSYSTEM.md`](https://github.com/vmcguire/BWA-Architecture/blob/main/ECOSYSTEM.md)
  — the full product map and the dual-surface / single-DSP architecture.
- [`docs/MARKET-PAIN-AND-ATTACKS.md`](https://github.com/vmcguire/BWA-Architecture/blob/main/docs/MARKET-PAIN-AND-ATTACKS.md)
  — what this plugin attacks (the pain it solves) and how.

## How this fits with the rest of BWA

BWA-Groove ships on **two surfaces** — same DSP, different UI:

1. **Standalone VST3** — drops into any DAW like a FabFilter / iZotope plugin.
   That's what this repo releases.
2. **Embedded cell inside BWA-Mix** — appears as a per-band / per-group cell
   processor inside BWA-Mix's track grid, sharing BWA-Mix's already-running
   band split and contributing to ecosystem-level cross-plugin features.

Both surfaces consume the **same authoritative DSP module**. Fix a bug once,
fixed everywhere.

## Status

🔴 Not built. Stub repo. Depends on shared/bar-timing/. Build target: Phase E4.

## Releases

Versioned `.vst3` builds for macOS land in this repo's
[Releases](https://github.com/vmcguire/BWA-Groove/releases). Build from
source if you want — see `CLAUDE.md` for the dev surface (it's not this repo).

## License

Proprietary. Distribution + license terms pending storefront launch — see
[BWA-Architecture/docs/GO-TO-MARKET.md](https://github.com/vmcguire/BWA-Architecture/blob/main/docs/GO-TO-MARKET.md).
