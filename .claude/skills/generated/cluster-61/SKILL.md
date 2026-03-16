---
name: cluster-61
description: "Skill for the Cluster_61 area of ice. 46 symbols across 10 files."
---

# Cluster_61

46 symbols | 10 files | Cohesion: 81%

## When to Use

- Working with code in `src/`
- Understanding how ice_vsi_init_vlan_ops, ice_ch_vsi_update_ring_vecs, ice_vsi_type_str work
- Modifying cluster_61-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_lib.c` | ice_vsi_type_str, ice_vsi_requires_vf, ice_get_free_slot, ice_vsi_delete_from_hw, ice_vsi_free_arrays (+26) |
| `src/ice_main.c` | ice_ch_vsi_map_rings_to_vecs, ice_ch_vsi_update_ring_vecs, ice_reinit_interrupt_scheme |
| `src/ice_base.h` | ice_vsi_alloc_q_vectors, ice_vsi_map_rings_to_vectors, ice_vsi_free_q_vectors |
| `src/ice.h` | ice_prepare_xdp_rings, ice_destroy_xdp_rings, ice_schedule_reset |
| `src/kcompat_impl.h` | krealloc_array |
| `src/ice_vsi_vlan_ops.h` | ice_vsi_init_vlan_ops |
| `src/ice_idc.c` | ice_cdev_info_request_reset |
| `src/ice_irq.h` | ice_init_interrupt_scheme |
| `src/ice_fltr.h` | ice_fltr_add_eth |
| `src/ice_ethtool.c` | ice_ethtool_reset |

## Entry Points

Start here when exploring this area:

- **`ice_vsi_init_vlan_ops`** (Function) — `src/ice_vsi_vlan_ops.h:25`
- **`ice_ch_vsi_update_ring_vecs`** (Function) — `src/ice_main.c:4235`
- **`ice_vsi_type_str`** (Function) — `src/ice_lib.c:36`
- **`ice_vsi_delete_from_hw`** (Function) — `src/ice_lib.c:405`
- **`ice_vsi_free_rss_global_lut`** (Function) — `src/ice_lib.c:475`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_vsi_init_vlan_ops` | Function | `src/ice_vsi_vlan_ops.h` | 25 |
| `ice_ch_vsi_update_ring_vecs` | Function | `src/ice_main.c` | 4235 |
| `ice_vsi_type_str` | Function | `src/ice_lib.c` | 36 |
| `ice_vsi_delete_from_hw` | Function | `src/ice_lib.c` | 405 |
| `ice_vsi_free_rss_global_lut` | Function | `src/ice_lib.c` | 475 |
| `ice_vsi_alloc_rss_global_lut` | Function | `src/ice_lib.c` | 502 |
| `ice_vsi_alloc_rss_lut` | Function | `src/ice_lib.c` | 584 |
| `ice_vsi_free` | Function | `src/ice_lib.c` | 777 |
| `ice_vsi_put_qs` | Function | `src/ice_lib.c` | 1124 |
| `ice_update_eth_stats` | Function | `src/ice_lib.c` | 2305 |
| `ice_vsi_cfg` | Function | `src/ice_lib.c` | 3398 |
| `ice_vsi_decfg` | Function | `src/ice_lib.c` | 3417 |
| `ice_vsi_setup` | Function | `src/ice_lib.c` | 3471 |
| `ice_vsi_release` | Function | `src/ice_lib.c` | 3818 |
| `ice_vsi_rebuild` | Function | `src/ice_lib.c` | 3989 |
| `ice_is_reset_in_progress` | Function | `src/ice_lib.c` | 4052 |
| `ice_wait_for_reset` | Function | `src/ice_lib.c` | 4073 |
| `ice_init_interrupt_scheme` | Function | `src/ice_irq.h` | 19 |
| `ice_fltr_add_eth` | Function | `src/ice_fltr.h` | 45 |
| `ice_vsi_alloc_q_vectors` | Function | `src/ice_base.h` | 13 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_vsi_setup → Ice_pf_to_dev` | intra_community | 5 |
| `Ice_vsi_setup → Min_t` | intra_community | 5 |
| `Ice_vsi_setup → Ice_vsi_alloc_rss_pf_lut` | intra_community | 4 |
| `Ice_vsi_setup → Ice_is_xdp_ena_vsi` | cross_community | 4 |
| `Ice_vsi_setup → Ice_destroy_xdp_rings` | intra_community | 4 |
| `Ice_vsi_rebuild → Ice_for_each_q_vector` | cross_community | 4 |
| `Ice_vsi_rebuild → Ice_for_each_alloc_txq` | cross_community | 4 |
| `Ice_vsi_rebuild → Ice_for_each_alloc_rxq` | cross_community | 4 |
| `Ice_vsi_rebuild → Ice_pf_to_dev` | intra_community | 4 |
| `Ice_vsi_rebuild → Min_t` | intra_community | 4 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 18 calls |
| Cluster_188 | 2 calls |
| Cluster_144 | 1 calls |
| Cluster_452 | 1 calls |
| Cluster_482 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_vsi_init_vlan_ops"})` — see callers and callees
2. `gitnexus_query({query: "cluster_61"})` — find related execution flows
3. Read key files listed above for implementation details
