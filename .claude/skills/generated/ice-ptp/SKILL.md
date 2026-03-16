---
name: ice-ptp
description: "Skill for the Ice_ptp_ area of ice. 35 symbols across 2 files."
---

# Ice_ptp_

35 symbols | 2 files | Cohesion: 75%

## When to Use

- Working with code in `src/`
- Understanding how ice_ptp_init_phc, ice_ptp_extts_event, ice_ptp_adj_clock work
- Modifying ice_ptp_-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_ptp.c` | ice_ptp_find_pin_idx, ice_ptp_extts_event, ice_ptp_cfg_extts, ice_ptp_disable_all_extts, ice_ptp_enable_all_extts (+19) |
| `src/ice_ptp_hw.c` | ice_ptp_cfg_sync_delay, ice_ptp_init_phc_e825c, ice_ptp_init_phc_e82x, ice_ptp_init_phc_e810, ice_ptp_init_phc_e830 (+6) |

## Entry Points

Start here when exploring this area:

- **`ice_ptp_init_phc`** (Function) — `src/ice_ptp_hw.c:5964`
- **`ice_ptp_extts_event`** (Function) — `src/ice_ptp.c:3547`
- **`ice_ptp_adj_clock`** (Function) — `src/ice_ptp_hw.c:5844`
- **`ice_ptp_phy_restart`** (Function) — `src/ice_ptp.c:3313`
- **`ice_ptp_process_ts`** (Function) — `src/ice_ptp.c:5197`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_ptp_init_phc` | Function | `src/ice_ptp_hw.c` | 5964 |
| `ice_ptp_extts_event` | Function | `src/ice_ptp.c` | 3547 |
| `ice_ptp_adj_clock` | Function | `src/ice_ptp_hw.c` | 5844 |
| `ice_ptp_phy_restart` | Function | `src/ice_ptp.c` | 3313 |
| `ice_ptp_process_ts` | Function | `src/ice_ptp.c` | 5197 |
| `ice_ptp_cfg_sync_delay` | Function | `src/ice_ptp_hw.c` | 463 |
| `ice_ptp_init_phc_e825c` | Function | `src/ice_ptp_hw.c` | 480 |
| `ice_ptp_init_phc_e82x` | Function | `src/ice_ptp_hw.c` | 2677 |
| `ice_ptp_init_phc_e810` | Function | `src/ice_ptp_hw.c` | 4396 |
| `ice_ptp_init_phc_e830` | Function | `src/ice_ptp_hw.c` | 4797 |
| `ice_ptp_find_pin_idx` | Function | `src/ice_ptp.c` | 1918 |
| `ice_ptp_cfg_extts` | Function | `src/ice_ptp.c` | 3601 |
| `ice_ptp_disable_all_extts` | Function | `src/ice_ptp.c` | 3684 |
| `ice_ptp_enable_all_extts` | Function | `src/ice_ptp.c` | 3700 |
| `ice_ptp_gpio_enable` | Function | `src/ice_ptp.c` | 3990 |
| `ice_ptp_prep_port_adj_e82x` | Function | `src/ice_ptp_hw.c` | 2759 |
| `ice_ptp_prep_phy_adj_e82x` | Function | `src/ice_ptp_hw.c` | 2806 |
| `ice_ptp_prep_phy_adj_ll_e810` | Function | `src/ice_ptp_hw.c` | 4458 |
| `ice_ptp_prep_phy_adj_e810` | Function | `src/ice_ptp_hw.c` | 4509 |
| `ice_ptp_is_managed_phy` | Function | `src/ice_ptp.c` | 1937 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_ptp_ts_irq → Ptp_port_to_pf` | cross_community | 6 |
| `Ice_ptp_ts_irq → Ice_pf_to_dev` | cross_community | 6 |
| `Ice_ptp_ts_irq → BIT_ULL` | cross_community | 6 |
| `Ice_ptp_update_incval → Ice_ptp_find_pin_idx` | cross_community | 4 |
| `Ice_ptp_ts_irq → ICE_GET_QUAD_NUM` | cross_community | 4 |
| `Ice_ptp_adj_clock → Wr32` | intra_community | 4 |
| `Ice_ptp_adj_clock → FIELD_PREP` | intra_community | 4 |
| `Ice_ptp_adj_clock → FIELD_GET` | intra_community | 4 |
| `Ice_ptp_adj_clock → Lower_16_bits` | cross_community | 4 |
| `Ice_ptp_adj_clock → Upper_16_bits` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 4 calls |
| Cluster_33 | 2 calls |
| Cluster_32 | 1 calls |
| Cluster_40 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_ptp_init_phc"})` — see callers and callees
2. `gitnexus_query({query: "ice_ptp_"})` — find related execution flows
3. Read key files listed above for implementation details
