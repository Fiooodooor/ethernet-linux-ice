---
name: ice-a
description: "Skill for the Ice_a area of ice. 25 symbols across 2 files."
---

# Ice_a

25 symbols | 2 files | Cohesion: 94%

## When to Use

- Working with code in `src/`
- Understanding how ice_acl_create_scen, ice_aq_alloc_acl_scen, ice_acl_add_entry work
- Modifying ice_a-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_acl_ctrl.c` | ice_acl_init_entry, ice_acl_tbl_calc_end_idx, ice_acl_alloc_partition, ice_acl_fill_tcam_select, ice_acl_set_scen_chnk_msk (+13) |
| `src/ice_acl.h` | ice_aq_alloc_acl_scen, ice_aq_program_acl_entry, ice_aq_program_actpair, ice_aq_alloc_acl_tbl, ice_aq_dealloc_acl_tbl (+2) |

## Entry Points

Start here when exploring this area:

- **`ice_acl_create_scen`** (Function) — `src/ice_acl_ctrl.c:734`
- **`ice_aq_alloc_acl_scen`** (Function) — `src/ice_acl.h:180`
- **`ice_acl_add_entry`** (Function) — `src/ice_acl_ctrl.c:962`
- **`ice_acl_prog_act`** (Function) — `src/ice_acl_ctrl.c:1037`
- **`ice_acl_rem_entry`** (Function) — `src/ice_acl_ctrl.c:1095`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_acl_create_scen` | Function | `src/ice_acl_ctrl.c` | 734 |
| `ice_aq_alloc_acl_scen` | Function | `src/ice_acl.h` | 180 |
| `ice_acl_add_entry` | Function | `src/ice_acl_ctrl.c` | 962 |
| `ice_acl_prog_act` | Function | `src/ice_acl_ctrl.c` | 1037 |
| `ice_acl_rem_entry` | Function | `src/ice_acl_ctrl.c` | 1095 |
| `ice_aq_program_acl_entry` | Function | `src/ice_acl.h` | 139 |
| `ice_aq_program_actpair` | Function | `src/ice_acl.h` | 151 |
| `ice_acl_create_tbl` | Function | `src/ice_acl_ctrl.c` | 302 |
| `ice_aq_alloc_acl_tbl` | Function | `src/ice_acl.h` | 133 |
| `ice_acl_destroy_tbl` | Function | `src/ice_acl_ctrl.c` | 885 |
| `ice_aq_dealloc_acl_tbl` | Function | `src/ice_acl.h` | 136 |
| `ice_aq_update_acl_scen` | Function | `src/ice_acl.h` | 185 |
| `ice_aq_query_acl_scen` | Function | `src/ice_acl.h` | 188 |
| `ice_acl_init_entry` | Function | `src/ice_acl_ctrl.c` | 20 |
| `ice_acl_tbl_calc_end_idx` | Function | `src/ice_acl_ctrl.c` | 96 |
| `ice_acl_alloc_partition` | Function | `src/ice_acl_ctrl.c` | 421 |
| `ice_acl_fill_tcam_select` | Function | `src/ice_acl_ctrl.c` | 558 |
| `ice_acl_set_scen_chnk_msk` | Function | `src/ice_acl_ctrl.c` | 615 |
| `ice_acl_assign_act_mem_for_scen` | Function | `src/ice_acl_ctrl.c` | 660 |
| `ice_acl_commit_partition` | Function | `src/ice_acl_ctrl.c` | 687 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_acl_create_scen"})` — see callers and callees
2. `gitnexus_query({query: "ice_a"})` — find related execution flows
3. Read key files listed above for implementation details
