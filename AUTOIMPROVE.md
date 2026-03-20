# AutoImprove - [Workspace Name]

## Phase
exploration | convergence | manual

## Objective Metric
| Metric | Target | Current |
|--------|--------|---------|
| [metric_name] | [target_value] | [current_value] |

## Measurement
| Tool | Frequency | Last Run |
|------|-----------|----------|
| [tool/script/name] | [interval] | [timestamp] |

## Lever (What Can Change)
| File/Directory | Editable | Last Modified |
|----------------|----------|---------------|
| CLAUDE.md | yes/no | [date] |
| CONTEXT.md | yes/no | [date] |
| [other_file] | yes/no | [date] |

## Log Routing
| Level | Destination | Filter |
|-------|-------------|--------|
| detail | ./autoimprove/logs/ | all |
| summary | ../autoimprove/summary.json | important |

## Decision Log
| Run | Change | Result | Keep? |
|-----|--------|--------|-------|
| | | | |

---

## How to Use

**1. Define what to optimize:**
Edit the Objective Metric table. Examples:
- `entropy` - project structure organization
- `routing_health` - CLAUDE.md routing freshness
- `test_coverage` - code test percentage
- `context_freshness` - days since CONTEXT.md updated

**2. Define how to measure:**
Point to a script, or use `manual` for human assessment.

**3. Define what can change:**
List files in the Lever table. Mark `yes` if agent can edit.

**4. Set phase:**
- `exploration` - auto-run every N minutes
- `convergence` - slower, more careful
- `manual` - agent proposes, human approves

**5. Run the skill:**
`/autoimprove` or invoke the autoimprove skill

---

## Example: Routing Health

```markdown
## Phase
exploration

## Objective Metric
| Metric | Target | Current |
|--------|--------|---------|
| routing_health | > 0.8 | 0.65 |

## Measurement
| Tool | Frequency | Last Run |
|------|-----------|----------|
| manual | daily | 2026-03-20 |

## Lever (What Can Change)
| File/Directory | Editable | Last Modified |
|----------------|----------|---------------|
| CLAUDE.md | yes | 2026-03-15 |
| CONTEXT.md | yes | 2026-03-18 |

## Decision Log
| Run | Change | Result | Keep? |
|-----|--------|--------|-------|
| 2026-03-20 10:00 | Added docs/ to routing | health 0.65→0.72 | ✓ |
```

---

**This file is where human intent meets AI capability.**
Both can edit. Both can propose. The feedback loop improves the workspace.