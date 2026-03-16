---
name: devlink
description: "Skill for the Devlink area of ice. 40 symbols across 4 files."
---

# Devlink

40 symbols | 4 files | Cohesion: 98%

## When to Use

- Working with code in `src/`
- Understanding how ice_devlink_register_resources, ice_devlink_unregister_resources, ice_devlink_register work
- Modifying devlink-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/kcompat_impl.h` | devl_lock, devl_unlock, devl_resource_register, devl_resources_unregister, devl_resource_occ_get_register (+10) |
| `src/ice_devlink.c` | ice_devlink_register_resources, ice_devlink_unregister_resources, ice_devlink_register, ice_devlink_unregister, ice_devlink_register_params (+7) |
| `src/devlink/health.c` | ice_deinit_devl_reporter, ice_health_deinit, ice_dump_ethtool_stats_to_fmsg, ice_devlink_health_report, ice_devlink_report_mdd_event (+5) |
| `src/ice_ethtool_common.h` | ice_get_strings, ice_get_sset_count, ice_get_ethtool_stats |

## Entry Points

Start here when exploring this area:

- **`ice_devlink_register_resources`** (Function) — `src/ice_devlink.c:1102`
- **`ice_devlink_unregister_resources`** (Function) — `src/ice_devlink.c:1189`
- **`ice_devlink_register`** (Function) — `src/ice_devlink.c:2300`
- **`ice_devlink_unregister`** (Function) — `src/ice_devlink.c:2328`
- **`ice_devlink_register_params`** (Function) — `src/ice_devlink.c:2349`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_devlink_register_resources` | Function | `src/ice_devlink.c` | 1102 |
| `ice_devlink_unregister_resources` | Function | `src/ice_devlink.c` | 1189 |
| `ice_devlink_register` | Function | `src/ice_devlink.c` | 2300 |
| `ice_devlink_unregister` | Function | `src/ice_devlink.c` | 2328 |
| `ice_devlink_register_params` | Function | `src/ice_devlink.c` | 2349 |
| `ice_devlink_unregister_params` | Function | `src/ice_devlink.c` | 2385 |
| `ice_devlink_destroy_pf_port` | Function | `src/ice_devlink.c` | 2519 |
| `ice_devlink_destroy_vf_port` | Function | `src/ice_devlink.c` | 2582 |
| `ice_devlink_init_regions` | Function | `src/ice_devlink.c` | 2840 |
| `ice_devlink_destroy_regions` | Function | `src/ice_devlink.c` | 2880 |
| `ice_devlink_tc_params_register` | Function | `src/ice_devlink.c` | 3380 |
| `ice_devlink_tc_params_unregister` | Function | `src/ice_devlink.c` | 3422 |
| `ice_health_deinit` | Function | `src/devlink/health.c` | 282 |
| `ice_get_strings` | Function | `src/ice_ethtool_common.h` | 6 |
| `ice_get_sset_count` | Function | `src/ice_ethtool_common.h` | 7 |
| `ice_get_ethtool_stats` | Function | `src/ice_ethtool_common.h` | 8 |
| `ice_devlink_report_mdd_event` | Function | `src/devlink/health.c` | 101 |
| `ice_report_tx_hang` | Function | `src/devlink/health.c` | 209 |
| `ice_health_init` | Function | `src/devlink/health.c` | 258 |
| `ice_health_clear` | Function | `src/devlink/health.c` | 303 |

## How to Explore

1. `gitnexus_context({name: "ice_devlink_register_resources"})` — see callers and callees
2. `gitnexus_query({query: "devlink"})` — find related execution flows
3. Read key files listed above for implementation details
