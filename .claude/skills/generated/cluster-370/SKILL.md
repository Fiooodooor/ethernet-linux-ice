---
name: cluster-370
description: "Skill for the Cluster_370 area of ice. 104 symbols across 4 files."
---

# Cluster_370

104 symbols | 4 files | Cohesion: 78%

## When to Use

- Working with code in `src/`
- Understanding how ice_get_initial_sw_cfg, ice_init_chk_subscribable_recipe_support, ice_init_def_sw_recp work
- Modifying cluster_370-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_common.c` | ice_dump_phy_type, ice_set_mac_type, ice_clear_pf_cfg, ice_aq_manage_mac_read, ice_phy_maps_to_media (+89) |
| `src/ice_sched.h` | ice_sched_init_port, ice_sched_query_res_alloc, ice_sched_get_psm_clk_freq, ice_cfg_rl_burst_size |
| `src/ice_switch.h` | ice_get_initial_sw_cfg, ice_init_chk_subscribable_recipe_support, ice_init_def_sw_recp |
| `src/ice_common.h` | ice_create_all_ctrlq, ice_check_sq_alive, ice_fill_dflt_direct_cmd_desc |

## Entry Points

Start here when exploring this area:

- **`ice_get_initial_sw_cfg`** (Function) — `src/ice_switch.h:436`
- **`ice_init_chk_subscribable_recipe_support`** (Function) — `src/ice_switch.h:534`
- **`ice_init_def_sw_recp`** (Function) — `src/ice_switch.h:560`
- **`ice_sched_init_port`** (Function) — `src/ice_sched.h:147`
- **`ice_sched_query_res_alloc`** (Function) — `src/ice_sched.h:151`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_get_initial_sw_cfg` | Function | `src/ice_switch.h` | 436 |
| `ice_init_chk_subscribable_recipe_support` | Function | `src/ice_switch.h` | 534 |
| `ice_init_def_sw_recp` | Function | `src/ice_switch.h` | 560 |
| `ice_sched_init_port` | Function | `src/ice_sched.h` | 147 |
| `ice_sched_query_res_alloc` | Function | `src/ice_sched.h` | 151 |
| `ice_sched_get_psm_clk_freq` | Function | `src/ice_sched.h` | 152 |
| `ice_cfg_rl_burst_size` | Function | `src/ice_sched.h` | 292 |
| `ice_create_all_ctrlq` | Function | `src/ice_common.h` | 58 |
| `ice_check_sq_alive` | Function | `src/ice_common.h` | 143 |
| `ice_fill_dflt_direct_cmd_desc` | Function | `src/ice_common.h` | 145 |
| `ice_clear_pf_cfg` | Function | `src/ice_common.c` | 216 |
| `ice_aq_get_phy_equalization` | Function | `src/ice_common.c` | 490 |
| `ice_aq_set_mac_cfg` | Function | `src/ice_common.c` | 749 |
| `ice_print_rollback_msg` | Function | `src/ice_common.c` | 895 |
| `ice_init_hw` | Function | `src/ice_common.c` | 985 |
| `ice_check_reset` | Function | `src/ice_common.c` | 1185 |
| `ice_reset` | Function | `src/ice_common.c` | 1305 |
| `ice_aq_send_cmd` | Function | `src/ice_common.c` | 2007 |
| `ice_aq_get_fw_ver` | Function | `src/ice_common.c` | 2065 |
| `ice_aq_send_driver_ver` | Function | `src/ice_common.c` | 2100 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_add_mac_with_counter → Ice_fill_dflt_direct_cmd_desc` | cross_community | 6 |
| `Ice_add_mac_with_sw_marker → Ice_fill_dflt_direct_cmd_desc` | cross_community | 6 |
| `Ice_init_hw → FIELD_GET` | intra_community | 5 |
| `Ice_init_hw → Rd32` | intra_community | 5 |
| `Ice_init_nvm → Ice_fill_dflt_direct_cmd_desc` | cross_community | 5 |
| `Ice_ena_vsi_txq → Ice_should_retry_sq_send_cmd` | cross_community | 5 |
| `Ice_ena_vsi_txq → Ice_sq_send_cmd` | cross_community | 5 |
| `Ice_ena_vsi_txq → Ice_vlock_fsleep` | cross_community | 5 |
| `Ice_init_hw → Wr32` | intra_community | 4 |
| `Ice_fwlog_init → Ice_fill_dflt_direct_cmd_desc` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 7 calls |
| Cluster_4 | 1 calls |
| Cluster_33 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_get_initial_sw_cfg"})` — see callers and callees
2. `gitnexus_query({query: "cluster_370"})` — find related execution flows
3. Read key files listed above for implementation details
