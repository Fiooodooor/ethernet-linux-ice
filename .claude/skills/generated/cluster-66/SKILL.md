---
name: cluster-66
description: "Skill for the Cluster_66 area of ice. 23 symbols across 6 files."
---

# Cluster_66

23 symbols | 6 files | Cohesion: 86%

## When to Use

- Working with code in `src/`
- Understanding how ice_repr_add_vf, ice_repr_rem_vf, ice_repr_start_tx_queues work
- Modifying cluster_66-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_eswitch.c` | ice_eswitch_setup_env, ice_eswitch_release_repr, ice_eswitch_setup_repr, ice_eswitch_update_repr, ice_eswitch_release_env (+8) |
| `src/ice_repr.h` | ice_repr_add_vf, ice_repr_rem_vf, ice_repr_start_tx_queues, ice_repr_stop_tx_queues |
| `src/ice_lib.h` | ice_vsi_update_security, ice_vsi_update_local_lb, ice_vsi_del_vlan_zero |
| `src/kcompat_impl.h` | radix_tree_empty |
| `src/ice_fltr.h` | ice_fltr_add_mac_and_broadcast |
| `src/ice_devlink.h` | ice_devlink_rate_clear_tx_topology |

## Entry Points

Start here when exploring this area:

- **`ice_repr_add_vf`** (Function) — `src/ice_repr.h:25`
- **`ice_repr_rem_vf`** (Function) — `src/ice_repr.h:26`
- **`ice_repr_start_tx_queues`** (Function) — `src/ice_repr.h:27`
- **`ice_repr_stop_tx_queues`** (Function) — `src/ice_repr.h:28`
- **`ice_vsi_update_security`** (Function) — `src/ice_lib.h:143`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_repr_add_vf` | Function | `src/ice_repr.h` | 25 |
| `ice_repr_rem_vf` | Function | `src/ice_repr.h` | 26 |
| `ice_repr_start_tx_queues` | Function | `src/ice_repr.h` | 27 |
| `ice_repr_stop_tx_queues` | Function | `src/ice_repr.h` | 28 |
| `ice_vsi_update_security` | Function | `src/ice_lib.h` | 143 |
| `ice_vsi_update_local_lb` | Function | `src/ice_lib.h` | 151 |
| `ice_vsi_del_vlan_zero` | Function | `src/ice_lib.h` | 157 |
| `ice_fltr_add_mac_and_broadcast` | Function | `src/ice_fltr.h` | 27 |
| `ice_eswitch_update_repr` | Function | `src/ice_eswitch.c` | 153 |
| `ice_eswitch_start_all_tx_queues` | Function | `src/ice_eswitch.c` | 412 |
| `ice_eswitch_stop_all_tx_queues` | Function | `src/ice_eswitch.c` | 433 |
| `ice_eswitch_attach` | Function | `src/ice_eswitch.c` | 460 |
| `ice_eswitch_detach` | Function | `src/ice_eswitch.c` | 513 |
| `ice_devlink_rate_clear_tx_topology` | Function | `src/ice_devlink.h` | 68 |
| `radix_tree_empty` | Function | `src/kcompat_impl.h` | 3417 |
| `ice_eswitch_setup_env` | Function | `src/ice_eswitch.c` | 19 |
| `ice_eswitch_release_repr` | Function | `src/ice_eswitch.c` | 92 |
| `ice_eswitch_setup_repr` | Function | `src/ice_eswitch.c` | 113 |
| `ice_eswitch_release_env` | Function | `src/ice_eswitch.c` | 255 |
| `ice_eswitch_enable_switchdev` | Function | `src/ice_eswitch.c` | 278 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_eswitch_attach → Test_and_set_bit` | intra_community | 4 |
| `Ice_eswitch_attach → Ice_down` | cross_community | 4 |
| `Ice_eswitch_attach → __dev_uc_unsync` | intra_community | 4 |
| `Ice_eswitch_attach → __dev_mc_unsync` | intra_community | 4 |
| `Ice_eswitch_attach → Ice_repr_stop_tx_queues` | intra_community | 4 |
| `Ice_eswitch_detach → Ice_repr_stop_tx_queues` | intra_community | 4 |
| `Ice_eswitch_detach → Ice_vsi_update_local_lb` | intra_community | 4 |
| `Ice_eswitch_detach → Ice_vsi_update_security` | intra_community | 4 |
| `Ice_eswitch_detach → Ice_fltr_add_mac_and_broadcast` | intra_community | 4 |
| `Ice_eswitch_attach → Ice_get_main_vsi` | cross_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 5 calls |
| Cluster_188 | 2 calls |

## How to Explore

1. `gitnexus_context({name: "ice_repr_add_vf"})` — see callers and callees
2. `gitnexus_query({query: "cluster_66"})` — find related execution flows
3. Read key files listed above for implementation details
