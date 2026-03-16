---
name: ice-ieps
description: "Skill for the Ice_ieps_ area of ice. 31 symbols across 3 files."
---

# Ice_ieps_

31 symbols | 3 files | Cohesion: 85%

## When to Use

- Working with code in `src/`
- Understanding how ice_ieps_entry, ice_ieps_init_lm_ops, ice_ieps_get_link_state_speed work
- Modifying ice_ieps_-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `src/ice_ieps.c` | ice_ieps_i2c_fill, ice_ieps_i2c_write, ice_ieps_i2c_read, ice_ieps_mdio_fill_desc, ice_ieps_mdio_read (+19) |
| `src/ice_ieps_lm.c` | ice_ieps_cpi_get_link_info, ice_ieps_cpi_set_port_cfg, ice_ieps_cpi_disable_port, ice_ieps_cpi_reset_port |
| `src/ice_ieps.h` | ice_ieps_init_lm_ops, ice_ieps_get_link_state_speed, ice_ieps_exec_cpi |

## Entry Points

Start here when exploring this area:

- **`ice_ieps_entry`** (Function) — `src/ice_ieps.c:1190`
- **`ice_ieps_init_lm_ops`** (Function) — `src/ice_ieps.h:21`
- **`ice_ieps_get_link_state_speed`** (Function) — `src/ice_ieps.h:16`
- **`ice_ieps_exec_cpi`** (Function) — `src/ice_ieps.h:19`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `ice_ieps_entry` | Function | `src/ice_ieps.c` | 1190 |
| `ice_ieps_init_lm_ops` | Function | `src/ice_ieps.h` | 21 |
| `ice_ieps_get_link_state_speed` | Function | `src/ice_ieps.h` | 16 |
| `ice_ieps_exec_cpi` | Function | `src/ice_ieps.h` | 19 |
| `ice_ieps_i2c_fill` | Function | `src/ice_ieps.c` | 44 |
| `ice_ieps_i2c_write` | Function | `src/ice_ieps.c` | 76 |
| `ice_ieps_i2c_read` | Function | `src/ice_ieps.c` | 129 |
| `ice_ieps_mdio_fill_desc` | Function | `src/ice_ieps.c` | 183 |
| `ice_ieps_mdio_read` | Function | `src/ice_ieps.c` | 236 |
| `ice_ieps_mdio_write` | Function | `src/ice_ieps.c` | 275 |
| `ice_ieps_gpio_fill_desc` | Function | `src/ice_ieps.c` | 317 |
| `ice_ieps_sw_gpio_set` | Function | `src/ice_ieps.c` | 346 |
| `ice_ieps_sw_gpio_get` | Function | `src/ice_ieps.c` | 377 |
| `ice_ieps_ver_check` | Function | `src/ice_ieps.c` | 413 |
| `ice_ieps_get_phy_status` | Function | `src/ice_ieps.c` | 493 |
| `ice_ieps_set_mode` | Function | `src/ice_ieps.c` | 536 |
| `ice_ieps_phy_reg_rw` | Function | `src/ice_ieps.c` | 885 |
| `ice_ieps_set_lesm` | Function | `src/ice_ieps.c` | 925 |
| `ice_ieps_set_link_mng` | Function | `src/ice_ieps.c` | 988 |
| `ice_ieps_get_phy_caps` | Function | `src/ice_ieps.c` | 438 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Ice_ieps_entry → Ice_pf_to_dev` | intra_community | 4 |
| `Ice_ieps_entry → Ice_ieps_i2c_fill` | intra_community | 3 |

## Connected Areas

| Area | Connections |
|------|-------------|
| Ice_ | 1 calls |

## How to Explore

1. `gitnexus_context({name: "ice_ieps_entry"})` — see callers and callees
2. `gitnexus_query({query: "ice_ieps_"})` — find related execution flows
3. Read key files listed above for implementation details
