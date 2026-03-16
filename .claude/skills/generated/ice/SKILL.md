---
name: ice
description: "Skill for the Ice_ area of ice. 1990 symbols across 105 files."
---

# Ice_

1990 symbols | 105 files | Cohesion: 72%

## When to Use

- Working with code in `src/`
- Understanding how ice_aq_get_sw_cfg, ice_dump_sw_cfg, ice_add_vsi work
- Modifying ice_-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_main.c` | ice_rem_all_chnl_fltrs, ice_get_devlink_port, ice_macvlan_vsi_setup, ice_lb_vsi_setup, ice_stop_eth (+188) |
| `src/ice_sched.c` | ice_sched_find_node_by_teid, ice_sched_add_node, ice_sched_get_first_node, ice_sched_get_tc_node, ice_sched_add_elems (+108) |
| `src/ice_flex_pipe.c` | ice_gen_key_word, ice_bits_max_set, ice_set_key, ice_tunnel_port_in_use_hlpr, ice_tunnel_port_in_use (+102) |
| `src/ice_ptp_hw.c` | ice_ptp_get_dest_dev_e825c, ice_write_phy_eth56g, ice_read_phy_eth56g, ice_write_port_eth56g, ice_write_xpcs_reg_eth56g (+88) |
| `src/ice_common.c` | ice_copy_rxq_ctx_to_hw, ice_write_rxq_ctx, ice_copy_tx_cmpltnq_ctx_to_hw, ice_write_tx_cmpltnq_ctx, ice_copy_tx_drbell_q_ctx_to_hw (+87) |
| `src/ice_virtchnl.c` | ice_vc_send_msg_to_vf, ice_vc_get_ver_msg, ice_vc_get_qos_caps, ice_vf_cfg_q_quanta_profile, ice_vc_cfg_q_quanta (+85) |
| `src/ice_switch.c` | ice_aq_get_sw_cfg, ice_dump_sw_cfg, ice_aq_add_vsi, ice_aq_free_vsi, ice_save_vsi_ctx (+72) |
| `src/ice.h` | ice_up, ice_netdev_to_pf, ice_init_aux_devices, ice_is_adq_active, ice_get_avail_txq_count (+72) |
| `src/ice_ddp.c` | ice_aq_upload_section, ice_aq_download_pkg, ice_get_pkg_seg_by_idx, ice_is_signing_seg_at_idx, ice_is_signing_seg_type_at_idx (+56) |
| `src/ice_lib.h` | ice_vsi_rebuild, ice_set_max_bw_limit, ice_vsi_setup, ice_free_res, ice_get_free_res_count (+55) |

## Entry Points

Start here when exploring this area:

- **`ice_aq_get_sw_cfg`** (Function) — `src/ice_switch.c:2265`
- **`ice_dump_sw_cfg`** (Function) — `src/ice_switch.c:2291`
- **`ice_add_vsi`** (Function) — `src/ice_switch.c:2810`
- **`ice_aq_get_vsi_params`** (Function) — `src/ice_switch.c:2934`
- **`ice_aq_add_recipe`** (Function) — `src/ice_switch.c:3082`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_aq_get_sw_cfg` | Function | `src/ice_switch.c` | 2265 |
| `ice_dump_sw_cfg` | Function | `src/ice_switch.c` | 2291 |
| `ice_add_vsi` | Function | `src/ice_switch.c` | 2810 |
| `ice_aq_get_vsi_params` | Function | `src/ice_switch.c` | 2934 |
| `ice_aq_add_recipe` | Function | `src/ice_switch.c` | 3082 |
| `ice_aq_get_recipe` | Function | `src/ice_switch.c` | 3119 |
| `ice_update_recipe_lkup_idx` | Function | `src/ice_switch.c` | 3159 |
| `ice_aq_map_recipe_to_profile` | Function | `src/ice_switch.c` | 3212 |
| `ice_aq_get_recipe_to_profile` | Function | `src/ice_switch.c` | 3238 |
| `ice_get_initial_sw_cfg` | Function | `src/ice_switch.c` | 3513 |
| `ice_aq_get_res_alloc` | Function | `src/ice_switch.c` | 4854 |
| `ice_aq_get_res_descs` | Function | `src/ice_switch.c` | 4891 |
| `ice_rem_adv_rule` | Function | `src/ice_switch.c` | 8737 |
| `ice_rem_adv_rule_by_id` | Function | `src/ice_switch.c` | 8835 |
| `ice_rem_adv_rule_for_vsi` | Function | `src/ice_switch.c` | 8871 |
| `ice_aq_read_nvm` | Function | `src/ice_nvm.c` | 21 |
| `ice_read_flat_nvm` | Function | `src/ice_nvm.c` | 65 |
| `ice_aq_update_nvm` | Function | `src/ice_nvm.c` | 142 |
| `ice_aq_erase_nvm` | Function | `src/ice_nvm.c` | 181 |
| `ice_acquire_nvm` | Function | `src/ice_nvm.c` | 242 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_init_pkg → Ice_find_buf_table` | cross_community | 8 |
| `Ice_start_phy_timer_eth56g → Lower_16_bits` | cross_community | 6 |
| `Ice_add_mac_with_counter → Ice_fill_eth_hdr` | cross_community | 6 |
| `Ice_add_mac_with_counter → Ice_fill_sw_info` | cross_community | 6 |
| `Ice_add_mac_with_counter → FIELD_PREP` | cross_community | 6 |
| `Ice_add_mac_with_counter → Ether_addr_copy` | cross_community | 6 |
| `Ice_add_mac_with_counter → Ice_fill_dflt_direct_cmd_desc` | cross_community | 6 |
| `Ice_init_nvm → Min_t` | cross_community | 6 |
| `Ice_init_nvm → Ice_acquire_res` | cross_community | 6 |
| `Ice_add_mac_with_sw_marker → Ice_fill_eth_hdr` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Cluster_370 | 54 calls |
| Cluster_188 | 39 calls |
| Ice_v | 20 calls |
| Ice_lag_ | 16 calls |
| Ice_sched_ | 13 calls |
| Cluster_430 | 11 calls |
| Cluster_267 | 11 calls |
| Cluster_33 | 10 calls |

## How to Explore

1. `gitnexus_context({name: "ice_aq_get_sw_cfg"})` — see callers and callees
2. `gitnexus_query({query: "ice_"})` — find related execution flows
3. Read key files listed above for implementation details
