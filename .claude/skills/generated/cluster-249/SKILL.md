---
name: cluster-249
description: "Skill for the Cluster_249 area of ice. 22 symbols across 3 files."
---

# Cluster_249

22 symbols | 3 files | Cohesion: 88%

## When to Use

- Working with code in `src/`
- Understanding how ice_tspll_monitor_lock_e825c, ice_tspll_cfg_cgu_err_reporting, ice_tspll_init work
- Modifying cluster_249-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_tspll.c` | tspll_cfg_store, tspll_cfg_show, ice_tspll_set_params_e82x, ice_tspll_clk_freq_str, ice_tspll_check_params (+15) |
| `src/ice_ptp.c` | dpll_ref_sw_store |
| `src/ice_lib.h` | ice_pf_state_is_nominal |

## Entry Points

Start here when exploring this area:

- **`ice_tspll_monitor_lock_e825c`** (Function) — `src/ice_tspll.c:715`
- **`ice_tspll_cfg_cgu_err_reporting`** (Function) — `src/ice_tspll.c:1162`
- **`ice_tspll_init`** (Function) — `src/ice_tspll.c:1182`
- **`ice_tspll_process_cgu_err`** (Function) — `src/ice_tspll.c:1237`
- **`ice_pf_state_is_nominal`** (Function) — `src/ice_lib.h:19`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_tspll_monitor_lock_e825c` | Function | `src/ice_tspll.c` | 715 |
| `ice_tspll_cfg_cgu_err_reporting` | Function | `src/ice_tspll.c` | 1162 |
| `ice_tspll_init` | Function | `src/ice_tspll.c` | 1182 |
| `ice_tspll_process_cgu_err` | Function | `src/ice_tspll.c` | 1237 |
| `ice_pf_state_is_nominal` | Function | `src/ice_lib.h` | 19 |
| `tspll_cfg_store` | Function | `src/ice_tspll.c` | 87 |
| `tspll_cfg_show` | Function | `src/ice_tspll.c` | 90 |
| `ice_tspll_set_params_e82x` | Function | `src/ice_tspll.c` | 139 |
| `ice_tspll_clk_freq_str` | Function | `src/ice_tspll.c` | 163 |
| `ice_tspll_check_params` | Function | `src/ice_tspll.c` | 190 |
| `ice_tspll_clk_src_str` | Function | `src/ice_tspll.c` | 246 |
| `ice_tspll_src_tmr_mode_str` | Function | `src/ice_tspll.c` | 264 |
| `ice_tspll_log_cfg` | Function | `src/ice_tspll.c` | 429 |
| `ice_tspll_cfg_e82x` | Function | `src/ice_tspll.c` | 449 |
| `ice_tspll_dis_sticky_bits_e82x` | Function | `src/ice_tspll.c` | 536 |
| `ice_tspll_cfg_e825c` | Function | `src/ice_tspll.c` | 556 |
| `ice_tspll_dis_sticky_bits_e825c` | Function | `src/ice_tspll.c` | 660 |
| `ice_tspll_lost_lock_e825c` | Function | `src/ice_tspll.c` | 676 |
| `ice_tspll_restart_e825c` | Function | `src/ice_tspll.c` | 694 |
| `ice_tspll_cfg` | Function | `src/ice_tspll.c` | 963 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_tspll_init → Ice_read_cgu_reg_or_die` | intra_community | 4 |
| `Ice_tspll_init → Ice_write_cgu_reg_or_die` | intra_community | 4 |
| `Ice_tspll_init → FIELD_GET` | intra_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Cluster_33 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_tspll_monitor_lock_e825c"})` — see callers and callees
2. `gitnexus_query({query: "cluster_249"})` — find related execution flows
3. Read key files listed above for implementation details
