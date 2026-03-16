---
name: adqsetup
description: "Skill for the Adqsetup area of ice. 136 symbols across 1 files."
---

# Adqsetup

136 symbols | 1 files | Cohesion: 81%

## When to Use

- Working with code in `scripts/`
- Understanding how sched_setaffinity, sendmsg, recvmsgs work
- Modifying adqsetup-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `scripts/adqsetup/adqsetup.py` | sched_setaffinity, _printhead, _mask, _readfile, _writefile (+131) |

## Entry Points

Start here when exploring this area:

- **`sched_setaffinity`** (Function) — `scripts/adqsetup/adqsetup.py:62`
- **`sendmsg`** (Function) — `scripts/adqsetup/adqsetup.py:1288`
- **`recvmsgs`** (Function) — `scripts/adqsetup/adqsetup.py:1296`
- **`send`** (Function) — `scripts/adqsetup/adqsetup.py:1313`
- **`addrs`** (Function) — `scripts/adqsetup/adqsetup.py:1474`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `StructTempl` | Class | `scripts/adqsetup/adqsetup.py` | 386 |
| `FeaturesGetBlock` | Class | `scripts/adqsetup/adqsetup.py` | 483 |
| `FeaturesSetBlock` | Class | `scripts/adqsetup/adqsetup.py` | 487 |
| `RXnfcFlowExt` | Class | `scripts/adqsetup/adqsetup.py` | 491 |
| `RXnfcFlowAddr` | Class | `scripts/adqsetup/adqsetup.py` | 495 |
| `RXnfcFlow` | Class | `scripts/adqsetup/adqsetup.py` | 499 |
| `RXnfc` | Class | `scripts/adqsetup/adqsetup.py` | 504 |
| `Genlmsghdr` | Class | `scripts/adqsetup/adqsetup.py` | 1390 |
| `IFAddrmsg` | Class | `scripts/adqsetup/adqsetup.py` | 1461 |
| `IFInfomsg` | Class | `scripts/adqsetup/adqsetup.py` | 1466 |
| `TCmsg` | Class | `scripts/adqsetup/adqsetup.py` | 1764 |
| `NLAttr` | Class | `scripts/adqsetup/adqsetup.py` | 975 |
| `GNLAttr` | Class | `scripts/adqsetup/adqsetup.py` | 1334 |
| `GNLOps` | Class | `scripts/adqsetup/adqsetup.py` | 1354 |
| `GNLOAttr` | Class | `scripts/adqsetup/adqsetup.py` | 1357 |
| `IFLAttr` | Class | `scripts/adqsetup/adqsetup.py` | 1430 |
| `TCAttr` | Class | `scripts/adqsetup/adqsetup.py` | 1514 |
| `TCMQAttr` | Class | `scripts/adqsetup/adqsetup.py` | 1528 |
| `TCMQNestAttr` | Class | `scripts/adqsetup/adqsetup.py` | 1549 |
| `TCFLAttr` | Class | `scripts/adqsetup/adqsetup.py` | 1581 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Apply → _ioctl` | cross_community | 5 |
| `Apply → _readfile` | intra_community | 3 |
| `Apply → _writefile` | intra_community | 3 |
| `Apply → _log` | cross_community | 3 |

## How to Explore

1. `gitnexus_context({name: "sched_setaffinity"})` — see callers and callees
2. `gitnexus_query({query: "adqsetup"})` — find related execution flows
3. Read key files listed above for implementation details
