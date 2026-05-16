# Lockwood Framework

A RedM server framework built for serious roleplay. Not a collection of scripts bolted together — a ground-up ecosystem with a shared data layer, unified permission model, and consistent conventions across every resource.

---

## What's in the box

22 open resources across 4 phases:

**Foundation** — `lw-db` · `lw-shared` · `lw-controls-api`

**Core** — `lw-core`

**API** — `lw-characters-api` · `lw-time-api` · `lw-weather-api` · `lw-economy-api` · `lw-inventory-api` · `lw-skills-api` · `lw-reputation-api` · `lw-legal-api` · `lw-property-api` · `lw-business-api` · `lw-bounty-api` · `lw-government-api` · `lw-organizations-api` · `lw-clothing-api` · `lw-appearance-api` · `lw-horse-appearance-api`

**UI & World** — `lw-ui-core` · `lw-world-objects`

The framework gives you a database wrapper with forward-only migrations, a shared utility and enum library, a central input binding registry with conflict detection, player session and routing bucket management, and a full suite of data APIs covering everything from economy and inventory to organizations and legal systems. You build the gameplay on top.

---

## Design principles

- **No magic globals.** Every resource declares its dependencies explicitly via exports. Nothing leaks across resource boundaries.
- **Data layer, not gameplay.** The framework owns state. Your resources own behavior.
- **Consistent conventions.** One DB pattern, one controls pattern, one permission pattern. Learn it once, apply it everywhere.
- **Forward-only migrations.** Schema changes are tracked, ordered, and never run twice.
- **Built for RedM.** Not a FiveM port. Written specifically for `rdr3`, `fx_version 'cerulean'`, and the RedM native set.

---

## Getting started

Documentation lives at [lockwood-framework.github.io](https://lockwood-framework.github.io).

Resources must be started in dependency order. See the [build order reference](https://lockwood-framework.github.io/build-order) before touching your `server.cfg`.

---

## Compatibility

| Runtime | Support |
|---|---|
| RedM / CFX `cerulean` | ✅ |
| Lua 5.4 | ✅ |
| oxmysql | ✅ Required |
| FiveM / GTA V | ❌ Not supported |
| VORP / RSG / RedEM:RP | ❌ Standalone only |

Lockwood Framework is standalone. It does not wrap or depend on any existing RedM framework.

---

## License

All resources in this organization are released under the [Rangeland Public License v1.0](https://github.com/Lockwood-Framework/lw-db/blob/main/LICENSE) — use it, modify it, don't sell it, don't ship it.

---

<div align="center">
  <sub>Built by <a href="https://github.com/Morgrhim">Morgrhim</a> · RedM · © 2026</sub>
</div>
