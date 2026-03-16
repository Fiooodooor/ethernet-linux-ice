---
name: cluster-2
description: "Skill for the Cluster_2 area of ice. 115 symbols across 3 files."
---

# Cluster_2

115 symbols | 3 files | Cohesion: 96%

## When to Use

- Working with code in `src/`
- Understanding how xas_load, xas_destroy, xas_nomem work
- Modifying cluster_2-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/kcompat_xarray.c` | radix_tree_node_rcu_free, xa_lock_type, xas_lock_type, xas_unlock_type, xa_track_free (+77) |
| `src/kcompat_xarray.h` | xa_to_value, xa_is_value, xa_mk_internal, xa_to_internal, xa_is_internal (+27) |
| `src/kcompat_impl.h` | kmem_cache_alloc_lru |

## Entry Points

Start here when exploring this area:

- **`xas_load`** (Function) — `src/kcompat_xarray.c:288`
- **`xas_destroy`** (Function) — `src/kcompat_xarray.c:321`
- **`xas_nomem`** (Function) — `src/kcompat_xarray.c:351`
- **`xas_create_range`** (Function) — `src/kcompat_xarray.c:762`
- **`xas_store`** (Function) — `src/kcompat_xarray.c:833`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `xas_load` | Function | `src/kcompat_xarray.c` | 288 |
| `xas_destroy` | Function | `src/kcompat_xarray.c` | 321 |
| `xas_nomem` | Function | `src/kcompat_xarray.c` | 351 |
| `xas_create_range` | Function | `src/kcompat_xarray.c` | 762 |
| `xas_store` | Function | `src/kcompat_xarray.c` | 833 |
| `xas_get_mark` | Function | `src/kcompat_xarray.c` | 915 |
| `xas_set_mark` | Function | `src/kcompat_xarray.c` | 934 |
| `xas_clear_mark` | Function | `src/kcompat_xarray.c` | 963 |
| `xas_init_marks` | Function | `src/kcompat_xarray.c` | 997 |
| `xas_split_alloc` | Function | `src/kcompat_xarray.c` | 1075 |
| `xas_split` | Function | `src/kcompat_xarray.c` | 1126 |
| `xas_pause` | Function | `src/kcompat_xarray.c` | 1193 |
| `xas_find` | Function | `src/kcompat_xarray.c` | 1311 |
| `xas_find_marked` | Function | `src/kcompat_xarray.c` | 1380 |
| `xas_find_conflict` | Function | `src/kcompat_xarray.c` | 1470 |
| `xa_load` | Function | `src/kcompat_xarray.c` | 1530 |
| `__xa_erase` | Function | `src/kcompat_xarray.c` | 1564 |
| `xa_erase` | Function | `src/kcompat_xarray.c` | 1583 |
| `__xa_store` | Function | `src/kcompat_xarray.c` | 1610 |
| `xa_store` | Function | `src/kcompat_xarray.c` | 1647 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Xas_find_conflict → Xa_mk_internal` | intra_community | 6 |
| `Xas_find_conflict → Xa_is_internal` | cross_community | 6 |
| `Xa_get_mark → Xa_mk_internal` | intra_community | 6 |
| `Xa_find_after → Xa_is_internal` | cross_community | 6 |
| `Xa_find_after → Xa_mk_internal` | cross_community | 6 |
| `Xas_create_range → Xa_is_internal` | intra_community | 6 |
| `Xa_destroy → Node_marks` | intra_community | 5 |
| `Xa_destroy → XA_FLAGS_MARK` | intra_community | 5 |
| `Xas_find_conflict → XA_NODE_BUG_ON` | cross_community | 5 |
| `Xas_find_conflict → IS_ENABLED` | intra_community | 5 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Cluster_6 | 13 calls |
| Cluster_3 | 1 calls |

## How to Explore

1. `gitnexus_context({name: "xas_load"})` — see callers and callees
2. `gitnexus_query({query: "cluster_2"})` — find related execution flows
3. Read key files listed above for implementation details
