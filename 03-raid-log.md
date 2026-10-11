# 03 · RAID Log

**RAID** = **R**isks, **A**ssumptions, **I**ssues, **D**ependencies. It is reviewed weekly by the project team and summarised at every steering committee. Full log: [`data/raid-log.csv`](data/raid-log.csv).

## Risks
| ID | Risk | Rating | Owner | Mitigation | Status |
|----|------|:------:|-------|------------|--------|
| R01 | Older POS version cannot export data in the required format | 🔴 High | IT Lead | Test older version in pilot; vendor patch as fallback | Open |
| R04 | Data discrepancies reduce trust in reports | 🔴 High | Data Lead | Daily reconciliation against POS end-of-day report | Open |
| R02 | Go-live disrupts service during trading | 🟡 Medium | PM | Go-lives before opening; rollback plan per site | Mitigating |
| R03 | Site managers do not adopt dashboards | 🟡 Medium | Head of Ops | Area-manager champions; role-based training | Mitigating |
| R05 | December peak overlaps Wave 3 | 🟡 Medium | PM | Go-live freeze from mid-December | Closed |

## Assumptions
| ID | Assumption | How it was checked | Status |
|----|-----------|--------------------|--------|
| A01 | All sites have stable broadband | Site audit in Discovery | ✅ Validated |
| A02 | Site managers can be released for 1 hour of training | Agreed at steering committee | ✅ Validated |

## Issues
| ID | Issue | Owner | Resolution | Status |
|----|-------|-------|-----------|--------|
| I01 | Duplicate transactions after refunds at 2 pilot sites | Integration Lead | Connector fix, retested before Wave 1 | ✅ Resolved |
| I02 | Guest-feedback feed delayed 24 hours | Platform Vendor | Feed changed to hourly | ✅ Resolved |

## Dependencies
| ID | Dependency | Owner | Status |
|----|-----------|-------|--------|
| D01 | POS vendor API credentials per site | Procurement | Tracking — requested 2 weeks before each wave |
| D02 | Finance sign-off on revenue definitions | Finance Director | ✅ Complete (week 3) |

## How the RAID Log Is Used
- **Every risk has one owner** and a clear next action.
- **Issues are risks that have happened**: when a risk occurs, it moves to the Issues section.
- **Assumptions are tested early**, because an assumption that turns out to be wrong becomes a risk.
- The **top 3 risks** appear on every status report, so leadership always knows what could go wrong.
