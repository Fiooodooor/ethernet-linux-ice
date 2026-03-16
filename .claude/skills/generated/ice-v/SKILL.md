---
name: ice-v
description: "Skill for the Ice_v area of ice. 62 symbols across 5 files."
---

# Ice_v

62 symbols | 5 files | Cohesion: 68%

## When to Use

- Working with code in `src/`
- Understanding how ice_vf_has_no_qs_ena, ice_vsi_ctrl_one_rx_ring, ice_vc_isvalid_vsi_id work
- Modifying ice_v-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_virtchnl.c` | ice_vf_ena_txq_interrupt, ice_vf_ena_rxq_interrupt, ice_vf_vsi_ena_single_rxq, ice_vf_vsi_ena_single_txq, ice_vf_vsi_dis_single_rxq (+44) |
| `src/ice_virtchnl_fdir.c` | ice_vc_fdir_free_prof, ice_vc_fdir_free_prof_all, ice_vc_fdir_rem_prof, ice_vc_fdir_rem_prof_all, ice_vc_fdir_write_flow_prof (+3) |
| `src/ice_lib.h` | ice_vsi_num_non_zero_vlans, ice_vsi_cfg_single_rxq, ice_vsi_cfg_single_txq |
| `src/ice_vf_lib_private.h` | ice_vf_has_no_qs_ena |
| `src/ice_base.h` | ice_vsi_ctrl_one_rx_ring |

## Entry Points

Start here when exploring this area:

- **`ice_vf_has_no_qs_ena`** (Function) — `src/ice_vf_lib_private.h:33`
- **`ice_vsi_ctrl_one_rx_ring`** (Function) — `src/ice_base.h:10`
- **`ice_vc_isvalid_vsi_id`** (Function) — `src/ice_virtchnl.c:879`
- **`ice_vc_fdir_free_prof_all`** (Function) — `src/ice_virtchnl_fdir.c:292`
- **`ice_vc_fdir_rem_prof_all`** (Function) — `src/ice_virtchnl_fdir.c:1543`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_vf_has_no_qs_ena` | Function | `src/ice_vf_lib_private.h` | 33 |
| `ice_vsi_ctrl_one_rx_ring` | Function | `src/ice_base.h` | 10 |
| `ice_vc_isvalid_vsi_id` | Function | `src/ice_virtchnl.c` | 879 |
| `ice_vc_fdir_free_prof_all` | Function | `src/ice_virtchnl_fdir.c` | 292 |
| `ice_vc_fdir_rem_prof_all` | Function | `src/ice_virtchnl_fdir.c` | 1543 |
| `ice_vf_fdir_exit` | Function | `src/ice_virtchnl_fdir.c` | 4322 |
| `ice_vf_fdir_exit_all` | Function | `src/ice_virtchnl_fdir.c` | 4334 |
| `ice_vsi_num_non_zero_vlans` | Function | `src/ice_lib.h` | 159 |
| `ice_vsi_cfg_single_rxq` | Function | `src/ice_lib.h` | 23 |
| `ice_vsi_cfg_single_txq` | Function | `src/ice_lib.h` | 25 |
| `ice_vf_ena_txq_interrupt` | Function | `src/ice_virtchnl.c` | 2973 |
| `ice_vf_ena_rxq_interrupt` | Function | `src/ice_virtchnl.c` | 2996 |
| `ice_vf_vsi_ena_single_rxq` | Function | `src/ice_virtchnl.c` | 3025 |
| `ice_vf_vsi_ena_single_txq` | Function | `src/ice_virtchnl.c` | 3059 |
| `ice_vf_vsi_dis_single_rxq` | Function | `src/ice_virtchnl.c` | 3238 |
| `ice_vc_supported_queue_type` | Function | `src/ice_virtchnl.c` | 5927 |
| `ice_vf_get_tc_of_qid` | Function | `src/ice_virtchnl.c` | 5940 |
| `ice_vf_get_vsi_of_qid` | Function | `src/ice_virtchnl.c` | 5959 |
| `ice_vf_get_vsi_qid` | Function | `src/ice_virtchnl.c` | 5981 |
| `ice_vc_validate_qs_v2_msg` | Function | `src/ice_virtchnl.c` | 6006 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 33 calls |
| Cluster_0 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_vf_has_no_qs_ena"})` — see callers and callees
2. `gitnexus_query({query: "ice_v"})` — find related execution flows
3. Read key files listed above for implementation details
