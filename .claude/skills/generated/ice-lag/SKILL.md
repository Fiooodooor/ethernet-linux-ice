---
name: ice-lag
description: "Skill for the Ice_lag_ area of ice. 47 symbols across 1 files."
---

# Ice_lag_

47 symbols | 1 files | Cohesion: 67%

## When to Use

- Working with code in `src/`
- Understanding how ice_lag_move_vf_nodes_cfg, ice_lag_prepare_vf_reset, ice_lag_complete_vf_reset work
- Modifying ice_lag_-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_lag.c` | ice_lag_find_hw_by_lport, ice_lag_qbuf_recfg, ice_lag_get_sched_parent, ice_lag_move_vf_node_tc, ice_lag_reclaim_vf_tc (+42) |

## Entry Points

Start here when exploring this area:

- **`ice_lag_move_vf_nodes_cfg`** (Function) — `src/ice_lag.c:1173`
- **`ice_lag_prepare_vf_reset`** (Function) — `src/ice_lag.c:1190`
- **`ice_lag_complete_vf_reset`** (Function) — `src/ice_lag.c:1224`
- **`ice_lag_sriov_aa_failover`** (Function) — `src/ice_lag.c:1569`
- **`ice_lag_rebuild`** (Function) — `src/ice_lag.c:4155`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_lag_move_vf_nodes_cfg` | Function | `src/ice_lag.c` | 1173 |
| `ice_lag_prepare_vf_reset` | Function | `src/ice_lag.c` | 1190 |
| `ice_lag_complete_vf_reset` | Function | `src/ice_lag.c` | 1224 |
| `ice_lag_sriov_aa_failover` | Function | `src/ice_lag.c` | 1569 |
| `ice_lag_rebuild` | Function | `src/ice_lag.c` | 4155 |
| `ice_lag_rdma_aa_failover` | Function | `src/ice_lag.c` | 2711 |
| `ice_lag_find_hw_by_lport` | Function | `src/ice_lag.c` | 96 |
| `ice_lag_qbuf_recfg` | Function | `src/ice_lag.c` | 761 |
| `ice_lag_get_sched_parent` | Function | `src/ice_lag.c` | 803 |
| `ice_lag_move_vf_node_tc` | Function | `src/ice_lag.c` | 975 |
| `ice_lag_reclaim_vf_tc` | Function | `src/ice_lag.c` | 1598 |
| `ice_lag_reclaim_vf_nodes` | Function | `src/ice_lag.c` | 1695 |
| `ice_lag_add_prune_list` | Function | `src/ice_lag.c` | 2421 |
| `ice_lag_del_prune_list` | Function | `src/ice_lag.c` | 2459 |
| `ice_lag_monitor_link` | Function | `src/ice_lag.c` | 2900 |
| `ice_lag_sriov_unregister` | Function | `src/ice_lag.c` | 3021 |
| `ice_lag_move_vf_nodes_tc_sync` | Function | `src/ice_lag.c` | 3900 |
| `ice_lag_move_vf_nodes_sync` | Function | `src/ice_lag.c` | 3997 |
| `ice_lag_move_single_vf_nodes` | Function | `src/ice_lag.c` | 1129 |
| `ice_lag_move_vf_nodes` | Function | `src/ice_lag.c` | 1145 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_lag_rebuild → Netif_is_ice` | cross_community | 5 |
| `Ice_lag_rebuild → Struct_size` | intra_community | 4 |
| `Ice_lag_rebuild → Ice_pf_to_dev` | intra_community | 4 |
| `Ice_lag_process_event → Ice_pf_to_dev` | cross_community | 4 |
| `Ice_lag_process_event → ICE_SW_RULE_VSI_LIST_SIZE` | cross_community | 4 |
| `Ice_lag_process_event → Struct_size` | cross_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Cluster_498 | 5 calls |
| Ice_ | 5 calls |
| Cluster_188 | 1 calls |
| Cluster_497 | 1 calls |
| Cluster_430 | 1 calls |
| Cluster_66 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_lag_move_vf_nodes_cfg"})` — see callers and callees
2. `gitnexus_query({query: "ice_lag_"})` — find related execution flows
3. Read key files listed above for implementation details
