---
name: cluster-33
description: "Skill for the Cluster_33 area of ice. 29 symbols across 6 files."
---

# Cluster_33

29 symbols | 6 files | Cohesion: 76%

## When to Use

- Working with code in `src/`
- Understanding how ice_get_ptp_src_clock_index, ice_ptp_src_cmd, ice_stop_phy_timer_eth56g work
- Modifying cluster_33-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_ptp_hw.c` | ice_get_ptp_src_clock_index, ice_ptp_tmr_cmd_to_src_reg, ice_ptp_src_cmd, ice_ptp_exec_tmr_cmd, ice_write_ptp_reg_eth56g (+14) |
| `src/ice_tspll.c` | ice_get_dest_cgu, ice_read_cgu_reg, ice_write_cgu_reg |
| `src/ice.h` | ice_is_dual, ice_is_primary, ice_get_primary_hw |
| `src/kcompat_impl.h` | ptp_read_system_prets, ptp_read_system_postts |
| `src/ice_ptp.c` | ice_ptp_read_src_clk_reg |
| `src/ice_common.c` | ice_get_phy_lane_number |

## Entry Points

Start here when exploring this area:

- **`ice_get_ptp_src_clock_index`** (Function) — `src/ice_ptp_hw.c:283`
- **`ice_ptp_src_cmd`** (Function) — `src/ice_ptp_hw.c:413`
- **`ice_stop_phy_timer_eth56g`** (Function) — `src/ice_ptp_hw.c:1933`
- **`ice_start_phy_timer_eth56g`** (Function) — `src/ice_ptp_hw.c:1960`
- **`ice_start_phy_timer_e82x`** (Function) — `src/ice_ptp_hw.c:3985`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_get_ptp_src_clock_index` | Function | `src/ice_ptp_hw.c` | 283 |
| `ice_ptp_src_cmd` | Function | `src/ice_ptp_hw.c` | 413 |
| `ice_stop_phy_timer_eth56g` | Function | `src/ice_ptp_hw.c` | 1933 |
| `ice_start_phy_timer_eth56g` | Function | `src/ice_ptp_hw.c` | 1960 |
| `ice_start_phy_timer_e82x` | Function | `src/ice_ptp_hw.c` | 3985 |
| `ice_ptp_lock` | Function | `src/ice_ptp_hw.c` | 5523 |
| `ice_ptp_unlock` | Function | `src/ice_ptp_hw.c` | 5552 |
| `ice_ptp_one_port_cmd` | Function | `src/ice_ptp_hw.c` | 5619 |
| `ice_ptp_write_incval_locked` | Function | `src/ice_ptp_hw.c` | 5817 |
| `ice_ptp_read_src_clk_reg` | Function | `src/ice_ptp.c` | 2103 |
| `ptp_read_system_prets` | Function | `src/kcompat_impl.h` | 1293 |
| `ptp_read_system_postts` | Function | `src/kcompat_impl.h` | 1296 |
| `ice_get_dest_cgu` | Function | `src/ice_tspll.c` | 324 |
| `ice_read_cgu_reg` | Function | `src/ice_tspll.c` | 348 |
| `ice_write_cgu_reg` | Function | `src/ice_tspll.c` | 389 |
| `ice_ptp_tmr_cmd_to_src_reg` | Function | `src/ice_ptp_hw.c` | 315 |
| `ice_ptp_exec_tmr_cmd` | Function | `src/ice_ptp_hw.c` | 432 |
| `ice_write_ptp_reg_eth56g` | Function | `src/ice_ptp_hw.c` | 645 |
| `ice_ptp_prep_port_adj_eth56g` | Function | `src/ice_ptp_hw.c` | 1207 |
| `ice_ptp_prep_phy_adj_eth56g` | Function | `src/ice_ptp_hw.c` | 1254 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_start_phy_timer_eth56g → Lower_16_bits` | cross_community | 6 |
| `Ice_ptp_update_incval → Ice_is_dual` | cross_community | 6 |
| `Ice_ptp_init → Ice_is_dual` | cross_community | 5 |
| `Ice_start_phy_timer_eth56g → Ice_phy_res_addr_eth56g` | cross_community | 5 |
| `Ice_start_phy_timer_eth56g → Upper_16_bits` | cross_community | 5 |
| `Ice_start_phy_timer_eth56g → Ice_sbq_rw_reg` | cross_community | 5 |
| `Ice_ptp_release → Ice_is_dual` | cross_community | 5 |
| `Ice_ptp_update_incval → Ice_get_primary_hw` | cross_community | 5 |
| `Ice_ptp_update_incval → Ptp_read_system_prets` | cross_community | 5 |
| `Ice_ptp_update_incval → Rd64` | cross_community | 5 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 18 calls |
| Ice_ptp_ | 1 calls |
| Cluster_370 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_get_ptp_src_clock_index"})` — see callers and callees
2. `gitnexus_query({query: "cluster_33"})` — find related execution flows
3. Read key files listed above for implementation details
