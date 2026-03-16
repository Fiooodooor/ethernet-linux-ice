---
name: cluster-144
description: "Skill for the Cluster_144 area of ice. 20 symbols across 5 files."
---

# Cluster_144

20 symbols | 5 files | Cohesion: 58%

## When to Use

- Working with code in `src/`
- Understanding how ice_vsi_set_inner_port_vlan, ice_vsi_ena_rx_vlan_filtering, ice_vsi_dis_rx_vlan_filtering work
- Modifying cluster_144-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_vsi_vlan_lib.c` | __ice_vsi_set_inner_port_vlan, ice_vsi_set_inner_port_vlan, ice_cfg_vlan_pruning, ice_vsi_ena_rx_vlan_filtering, ice_vsi_dis_rx_vlan_filtering (+8) |
| `src/ice_fw_update.c` | ice_send_package_data, ice_check_component_response, ice_send_component_table |
| `src/ice_ethtool.c` | ice_get_eeprom, ice_set_pauseparam |
| `src/ice_lib.c` | ice_set_link |
| `src/ice.h` | ice_aq_str |

## Entry Points

Start here when exploring this area:

- **`ice_vsi_set_inner_port_vlan`** (Function) — `src/ice_vsi_vlan_lib.c:253`
- **`ice_vsi_ena_rx_vlan_filtering`** (Function) — `src/ice_vsi_vlan_lib.c:323`
- **`ice_vsi_dis_rx_vlan_filtering`** (Function) — `src/ice_vsi_vlan_lib.c:328`
- **`ice_vsi_ena_outer_stripping`** (Function) — `src/ice_vsi_vlan_lib.c:418`
- **`ice_vsi_dis_outer_stripping`** (Function) — `src/ice_vsi_vlan_lib.c:476`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_vsi_set_inner_port_vlan` | Function | `src/ice_vsi_vlan_lib.c` | 253 |
| `ice_vsi_ena_rx_vlan_filtering` | Function | `src/ice_vsi_vlan_lib.c` | 323 |
| `ice_vsi_dis_rx_vlan_filtering` | Function | `src/ice_vsi_vlan_lib.c` | 328 |
| `ice_vsi_ena_outer_stripping` | Function | `src/ice_vsi_vlan_lib.c` | 418 |
| `ice_vsi_dis_outer_stripping` | Function | `src/ice_vsi_vlan_lib.c` | 476 |
| `ice_vsi_ena_outer_insertion` | Function | `src/ice_vsi_vlan_lib.c` | 527 |
| `ice_vsi_dis_outer_insertion` | Function | `src/ice_vsi_vlan_lib.c` | 583 |
| `ice_vsi_set_outer_port_vlan` | Function | `src/ice_vsi_vlan_lib.c` | 700 |
| `ice_vsi_clear_port_vlan` | Function | `src/ice_vsi_vlan_lib.c` | 712 |
| `ice_set_link` | Function | `src/ice_lib.c` | 4731 |
| `ice_aq_str` | Function | `src/ice.h` | 1822 |
| `__ice_vsi_set_inner_port_vlan` | Function | `src/ice_vsi_vlan_lib.c` | 216 |
| `ice_cfg_vlan_pruning` | Function | `src/ice_vsi_vlan_lib.c` | 275 |
| `tpid_to_vsi_outer_vlan_type` | Function | `src/ice_vsi_vlan_lib.c` | 379 |
| `__ice_vsi_set_outer_port_vlan` | Function | `src/ice_vsi_vlan_lib.c` | 639 |
| `ice_send_package_data` | Function | `src/ice_fw_update.c` | 56 |
| `ice_check_component_response` | Function | `src/ice_fw_update.c` | 102 |
| `ice_send_component_table` | Function | `src/ice_fw_update.c` | 216 |
| `ice_get_eeprom` | Function | `src/ice_ethtool.c` | 842 |
| `ice_set_pauseparam` | Function | `src/ice_ethtool.c` | 5208 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_vc_process_vf_msg → Ice_aq_str` | cross_community | 3 |

## How to Explore

1. `gitnexus_context({name: "ice_vsi_set_inner_port_vlan"})` — see callers and callees
2. `gitnexus_query({query: "cluster_144"})` — find related execution flows
3. Read key files listed above for implementation details
