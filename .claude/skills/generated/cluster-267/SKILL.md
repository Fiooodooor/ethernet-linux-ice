---
name: cluster-267
description: "Skill for the Cluster_267 area of ice. 31 symbols across 1 files."
---

# Cluster_267

31 symbols | 1 files | Cohesion: 76%

## When to Use

- Working with code in `src/`
- Understanding how ice_is_vsi_valid, ice_get_hw_vsi_num, ice_free_vsi work
- Modifying cluster_267-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_switch.c` | ice_aq_update_vsi, ice_is_vsi_valid, ice_get_hw_vsi_num, ice_free_vsi, ice_update_vsi (+26) |

## Entry Points

Start here when exploring this area:

- **`ice_is_vsi_valid`** (Function) — `src/ice_switch.c:2699`
- **`ice_get_hw_vsi_num`** (Function) — `src/ice_switch.c:2712`
- **`ice_free_vsi`** (Function) — `src/ice_switch.c:2851`
- **`ice_update_vsi`** (Function) — `src/ice_switch.c:2875`
- **`ice_mac_fltr_exist`** (Function) — `src/ice_switch.c:4928`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_is_vsi_valid` | Function | `src/ice_switch.c` | 2699 |
| `ice_get_hw_vsi_num` | Function | `src/ice_switch.c` | 2712 |
| `ice_free_vsi` | Function | `src/ice_switch.c` | 2851 |
| `ice_update_vsi` | Function | `src/ice_switch.c` | 2875 |
| `ice_mac_fltr_exist` | Function | `src/ice_switch.c` | 4928 |
| `ice_vlan_fltr_exist` | Function | `src/ice_switch.c` | 4976 |
| `ice_add_mac` | Function | `src/ice_switch.c` | 5200 |
| `ice_add_mac_vlan` | Function | `src/ice_switch.c` | 5450 |
| `ice_add_eth_mac` | Function | `src/ice_switch.c` | 5504 |
| `ice_cfg_dflt_vsi` | Function | `src/ice_switch.c` | 5710 |
| `ice_remove_mac` | Function | `src/ice_switch.c` | 5888 |
| `ice_set_vsi_promisc` | Function | `src/ice_switch.c` | 6466 |
| `ice_add_mac_with_sw_marker` | Function | `src/ice_switch.c` | 6783 |
| `ice_add_mac_with_counter` | Function | `src/ice_switch.c` | 6879 |
| `ice_aq_update_vsi` | Function | `src/ice_switch.c` | 2663 |
| `ice_update_vsi_list_rule` | Function | `src/ice_switch.c` | 4189 |
| `ice_find_rule_entry` | Function | `src/ice_switch.c` | 4528 |
| `ice_add_rule_internal` | Function | `src/ice_switch.c` | 4603 |
| `ice_remove_vsi_list_rule` | Function | `src/ice_switch.c` | 4653 |
| `ice_rem_update_vsi_list` | Function | `src/ice_switch.c` | 4671 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_add_mac_with_counter → Ice_fill_eth_hdr` | cross_community | 6 |
| `Ice_add_mac_with_counter → Ice_fill_sw_info` | cross_community | 6 |
| `Ice_add_mac_with_counter → FIELD_PREP` | cross_community | 6 |
| `Ice_add_mac_with_counter → Ether_addr_copy` | cross_community | 6 |
| `Ice_add_mac_with_counter → Ice_fill_dflt_direct_cmd_desc` | cross_community | 6 |
| `Ice_add_mac_with_sw_marker → Ice_fill_eth_hdr` | cross_community | 6 |
| `Ice_add_mac_with_sw_marker → Ice_fill_sw_info` | cross_community | 6 |
| `Ice_add_mac_with_sw_marker → FIELD_PREP` | cross_community | 6 |
| `Ice_add_mac_with_sw_marker → Ether_addr_copy` | cross_community | 6 |
| `Ice_add_mac_with_sw_marker → Ice_fill_dflt_direct_cmd_desc` | cross_community | 6 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 18 calls |
| Cluster_370 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_is_vsi_valid"})` — see callers and callees
2. `gitnexus_query({query: "cluster_267"})` — find related execution flows
3. Read key files listed above for implementation details
