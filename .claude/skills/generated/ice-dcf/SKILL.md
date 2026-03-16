---
name: ice-dcf
description: "Skill for the Ice_dcf_ area of ice. 20 symbols across 1 files."
---

# Ice_dcf_

20 symbols | 1 files | Cohesion: 84%

## When to Use

- Working with code in `src/`
- Understanding how ice_dcf_is_udp_tunnel_aq_cmd, ice_dcf_post_aq_send_cmd, ice_dcf_pre_aq_send_cmd work
- Modifying ice_dcf_-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_dcf.c` | ice_dcf_is_udp_tunnel_aq_cmd, ice_dcf_parse_alloc_vsi_list_res, ice_dcf_parse_free_vsi_list_res, ice_dcf_parse_add_sw_rule_data, ice_dcf_parse_rm_sw_rule_data (+15) |

## Entry Points

Start here when exploring this area:

- **`ice_dcf_is_udp_tunnel_aq_cmd`** (Function) — `src/ice_dcf.c:98`
- **`ice_dcf_post_aq_send_cmd`** (Function) — `src/ice_dcf.c:1026`
- **`ice_dcf_pre_aq_send_cmd`** (Function) — `src/ice_dcf.c:1130`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_dcf_is_udp_tunnel_aq_cmd` | Function | `src/ice_dcf.c` | 98 |
| `ice_dcf_post_aq_send_cmd` | Function | `src/ice_dcf.c` | 1026 |
| `ice_dcf_pre_aq_send_cmd` | Function | `src/ice_dcf.c` | 1130 |
| `ice_dcf_parse_alloc_vsi_list_res` | Function | `src/ice_dcf.c` | 622 |
| `ice_dcf_parse_free_vsi_list_res` | Function | `src/ice_dcf.c` | 648 |
| `ice_dcf_parse_add_sw_rule_data` | Function | `src/ice_dcf.c` | 741 |
| `ice_dcf_parse_rm_sw_rule_data` | Function | `src/ice_dcf.c` | 834 |
| `ice_dcf_handle_add_sw_rule_rsp` | Function | `src/ice_dcf.c` | 856 |
| `ice_dcf_handle_rm_sw_rule_rsp` | Function | `src/ice_dcf.c` | 905 |
| `ice_dcf_handle_alloc_res_rsp` | Function | `src/ice_dcf.c` | 925 |
| `ice_dcf_handle_free_res_rsp` | Function | `src/ice_dcf.c` | 946 |
| `ice_dcf_handle_udp_tunnel_rsp` | Function | `src/ice_dcf.c` | 968 |
| `ice_dcf_find_vsi_list_info` | Function | `src/ice_dcf.c` | 581 |
| `ice_dcf_add_vsi_id` | Function | `src/ice_dcf.c` | 598 |
| `ice_dcf_del_vsi_id` | Function | `src/ice_dcf.c` | 610 |
| `ice_dcf_set_vsi_list` | Function | `src/ice_dcf.c` | 678 |
| `ice_dcf_clear_vsi_list` | Function | `src/ice_dcf.c` | 701 |
| `ice_dcf_find_sw_rule` | Function | `src/ice_dcf.c` | 724 |
| `ice_dcf_parse_updt_sw_rule_data` | Function | `src/ice_dcf.c` | 767 |
| `ice_dcf_handle_updt_sw_rule_rsp` | Function | `src/ice_dcf.c` | 879 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_dcf_post_aq_send_cmd → Test_and_set_bit` | cross_community | 5 |
| `Ice_dcf_post_aq_send_cmd → Ice_dcf_find_vsi_list_info` | cross_community | 4 |
| `Ice_dcf_post_aq_send_cmd → FIELD_GET` | intra_community | 4 |
| `Ice_dcf_post_aq_send_cmd → Ice_dcf_find_sw_rule` | cross_community | 4 |
| `Ice_dcf_post_aq_send_cmd → Ice_pf_to_dev` | cross_community | 4 |

## How to Explore

1. `gitnexus_context({name: "ice_dcf_is_udp_tunnel_aq_cmd"})` — see callers and callees
2. `gitnexus_query({query: "ice_dcf_"})` — find related execution flows
3. Read key files listed above for implementation details
