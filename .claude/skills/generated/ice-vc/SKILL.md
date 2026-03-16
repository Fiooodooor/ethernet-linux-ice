---
name: ice-vc
description: "Skill for the Ice_vc_ area of ice. 26 symbols across 2 files."
---

# Ice_vc_

26 symbols | 2 files | Cohesion: 76%

## When to Use

- Working with code in `src/`
- Understanding how ice_vc_add_fdir_fltr, ice_vc_set_default_allowlist, ice_vc_set_working_allowlist work
- Modifying ice_vc_-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_virtchnl_fdir.c` | ice_vc_fdir_comp_rules, ice_vc_fdir_is_dup_fltr, ice_vc_fdir_insert_entry, ice_vc_fdir_add_del_raw, ice_vc_fdir_set_irq_ctx (+15) |
| `src/ice_virtchnl_allowlist.c` | ice_vc_allowlist_opcodes, ice_vc_clear_allowlist, ice_vc_set_default_allowlist, ice_vc_set_working_allowlist, ice_vc_set_hqos_allowlist (+1) |

## Entry Points

Start here when exploring this area:

- **`ice_vc_add_fdir_fltr`** (Function) — `src/ice_virtchnl_fdir.c:3985`
- **`ice_vc_set_default_allowlist`** (Function) — `src/ice_virtchnl_allowlist.c:215`
- **`ice_vc_set_working_allowlist`** (Function) — `src/ice_virtchnl_allowlist.c:229`
- **`ice_vc_set_hqos_allowlist`** (Function) — `src/ice_virtchnl_allowlist.c:242`
- **`ice_vc_set_caps_allowlist`** (Function) — `src/ice_virtchnl_allowlist.c:252`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_vc_add_fdir_fltr` | Function | `src/ice_virtchnl_fdir.c` | 3985 |
| `ice_vc_set_default_allowlist` | Function | `src/ice_virtchnl_allowlist.c` | 215 |
| `ice_vc_set_working_allowlist` | Function | `src/ice_virtchnl_allowlist.c` | 229 |
| `ice_vc_set_hqos_allowlist` | Function | `src/ice_virtchnl_allowlist.c` | 242 |
| `ice_vc_set_caps_allowlist` | Function | `src/ice_virtchnl_allowlist.c` | 252 |
| `ice_vc_del_fdir_fltr` | Function | `src/ice_virtchnl_fdir.c` | 4210 |
| `ice_vc_fdir_comp_rules` | Function | `src/ice_virtchnl_fdir.c` | 3107 |
| `ice_vc_fdir_is_dup_fltr` | Function | `src/ice_virtchnl_fdir.c` | 3128 |
| `ice_vc_fdir_insert_entry` | Function | `src/ice_virtchnl_fdir.c` | 3155 |
| `ice_vc_fdir_add_del_raw` | Function | `src/ice_virtchnl_fdir.c` | 3230 |
| `ice_vc_fdir_set_irq_ctx` | Function | `src/ice_virtchnl_fdir.c` | 3768 |
| `ice_vc_fdir_clear_irq_ctx` | Function | `src/ice_virtchnl_fdir.c` | 3806 |
| `ice_vc_parser_fv_check_diff` | Function | `src/ice_virtchnl_fdir.c` | 3827 |
| `ice_vc_parser_fv_save` | Function | `src/ice_virtchnl_fdir.c` | 3843 |
| `ice_vc_add_fdir_raw` | Function | `src/ice_virtchnl_fdir.c` | 3860 |
| `ice_vc_del_fdir_raw` | Function | `src/ice_virtchnl_fdir.c` | 4125 |
| `ice_vc_allowlist_opcodes` | Function | `src/ice_virtchnl_allowlist.c` | 193 |
| `ice_vc_clear_allowlist` | Function | `src/ice_virtchnl_allowlist.c` | 206 |
| `ice_vc_fdir_is_raw_flow` | Function | `src/ice_virtchnl_fdir.c` | 2195 |
| `ice_vc_fdir_parse_raw` | Function | `src/ice_virtchnl_fdir.c` | 2211 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_vc_add_fdir_fltr → Ice_pf_to_dev` | cross_community | 3 |
| `Ice_vc_add_fdir_fltr → Ice_vf_ctrl_vsi_setup` | cross_community | 3 |
| `Ice_vc_add_fdir_fltr → Ice_vsi_open_ctrl` | cross_community | 3 |
| `Ice_vc_add_fdir_fltr → Ice_vsi_release` | cross_community | 3 |
| `Ice_vc_del_fdir_fltr → Ice_pf_to_dev` | cross_community | 3 |
| `Ice_vc_del_fdir_fltr → Timer_setup` | cross_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 5 calls |
| Ice_vc_fdir_ | 1 calls |
| Ice_v | 1 calls |
| Cluster_188 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_vc_add_fdir_fltr"})` — see callers and callees
2. `gitnexus_query({query: "ice_vc_"})` — find related execution flows
3. Read key files listed above for implementation details
