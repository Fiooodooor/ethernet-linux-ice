---
name: ice-dpll
description: "Skill for the Ice_dpll_ area of ice. 78 symbols across 1 files."
---

# Ice_dpll_

78 symbols | 1 files | Cohesion: 68%

## When to Use

- Working with code in `src/`
- Understanding how ice_dpll_deinit, ice_dpll_init, ice_dpll_pin_update_unlock work
- Modifying ice_dpll_-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_dpll.c` | ice_dpll_is_pps_phase_monitor, ice_dpll_update_state, ice_dpll_deinit_dpll, ice_dpll_init_dpll, ice_dpll_deinit_worker (+73) |

## Entry Points

Start here when exploring this area:

- **`ice_dpll_deinit`** (Function) — `src/ice_dpll.c:3841`
- **`ice_dpll_init`** (Function) — `src/ice_dpll.c:3956`
- **`ice_dpll_pin_update_unlock`** (Function) — `src/ice_dpll.c:4000`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_dpll_deinit` | Function | `src/ice_dpll.c` | 3841 |
| `ice_dpll_init` | Function | `src/ice_dpll.c` | 3956 |
| `ice_dpll_pin_update_unlock` | Function | `src/ice_dpll.c` | 4000 |
| `ice_dpll_is_pps_phase_monitor` | Function | `src/ice_dpll.c` | 2493 |
| `ice_dpll_update_state` | Function | `src/ice_dpll.c` | 2600 |
| `ice_dpll_deinit_dpll` | Function | `src/ice_dpll.c` | 3141 |
| `ice_dpll_init_dpll` | Function | `src/ice_dpll.c` | 3163 |
| `ice_dpll_deinit_worker` | Function | `src/ice_dpll.c` | 3206 |
| `ice_dpll_init_worker` | Function | `src/ice_dpll.c` | 3252 |
| `ice_dpll_deinit_info` | Function | `src/ice_dpll.c` | 3614 |
| `ice_dpll_init_info` | Function | `src/ice_dpll.c` | 3742 |
| `ice_dpll_init_unmanaged` | Function | `src/ice_dpll.c` | 3865 |
| `ice_dpll_init_managed` | Function | `src/ice_dpll.c` | 3905 |
| `ice_dpll_is_reset` | Function | `src/ice_dpll.c` | 109 |
| `ice_dpll_hw_input_prio_set` | Function | `src/ice_dpll.c` | 756 |
| `ice_dpll_input_prio_set` | Function | `src/ice_dpll.c` | 1453 |
| `ice_dpll_sw_input_prio_set` | Function | `src/ice_dpll.c` | 1492 |
| `ice_dpll_pin_sw_direction_get` | Function | `src/ice_dpll.c` | 1616 |
| `ice_dpll_output_esync_set` | Function | `src/ice_dpll.c` | 1934 |
| `ice_dpll_output_esync_get` | Function | `src/ice_dpll.c` | 1989 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Cluster_144 | 10 calls |
| Ice_ | 7 calls |
| Cluster_188 | 2 calls |

## How to Explore

1. `gitnexus_context({name: "ice_dpll_deinit"})` — see callers and callees
2. `gitnexus_query({query: "ice_dpll_"})` — find related execution flows
3. Read key files listed above for implementation details
