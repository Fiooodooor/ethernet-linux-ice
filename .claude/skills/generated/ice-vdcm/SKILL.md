---
name: ice-vdcm
description: "Skill for the Ice_vdcm_ area of ice. 23 symbols across 1 files."
---

# Ice_vdcm_

23 symbols | 1 files | Cohesion: 96%

## When to Use

- Working with code in `src/`
- Understanding how ice_vdcm_zap work
- Modifying ice_vdcm_-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_vdcm.c` | ice_vdcm_cfg_read, ice_vdcm_cfg_write_mask, ice_vdcm_cfg_write_bar, ice_vdcm_cfg_write, ice_vdcm_bar0_read (+18) |

## Entry Points

Start here when exploring this area:

- **`ice_vdcm_zap`** (Function) — `src/ice_vdcm.c:1261`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_vdcm_zap` | Function | `src/ice_vdcm.c` | 1261 |
| `ice_vdcm_cfg_read` | Function | `src/ice_vdcm.c` | 154 |
| `ice_vdcm_cfg_write_mask` | Function | `src/ice_vdcm.c` | 189 |
| `ice_vdcm_cfg_write_bar` | Function | `src/ice_vdcm.c` | 228 |
| `ice_vdcm_cfg_write` | Function | `src/ice_vdcm.c` | 273 |
| `ice_vdcm_bar0_read` | Function | `src/ice_vdcm.c` | 305 |
| `ice_vdcm_bar0_write` | Function | `src/ice_vdcm.c` | 329 |
| `ice_vdcm_rw` | Function | `src/ice_vdcm.c` | 354 |
| `ice_vdcm_read` | Function | `src/ice_vdcm.c` | 394 |
| `ice_vdcm_write` | Function | `src/ice_vdcm.c` | 462 |
| `ice_vdcm_vfio_device_get_info` | Function | `src/ice_vdcm.c` | 526 |
| `ice_vdcm_sparse_mmap_cap` | Function | `src/ice_vdcm.c` | 554 |
| `ice_vdcm_vfio_device_get_region_info` | Function | `src/ice_vdcm.c` | 773 |
| `ice_vdcm_vfio_device_get_irq_info` | Function | `src/ice_vdcm.c` | 854 |
| `ice_vdcm_vfio_device_reset` | Function | `src/ice_vdcm.c` | 1343 |
| `ice_vdcm_ioctl` | Function | `src/ice_vdcm.c` | 1359 |
| `ice_vdcm_set_vector_signal` | Function | `src/ice_vdcm.c` | 911 |
| `ice_vdcm_set_vector_signals` | Function | `src/ice_vdcm.c` | 989 |
| `ice_vdcm_msix_enable` | Function | `src/ice_vdcm.c` | 1021 |
| `ice_vdcm_msix_disable` | Function | `src/ice_vdcm.c` | 1040 |

## How to Explore

1. `gitnexus_context({name: "ice_vdcm_zap"})` — see callers and callees
2. `gitnexus_query({query: "ice_vdcm_"})` — find related execution flows
3. Read key files listed above for implementation details
