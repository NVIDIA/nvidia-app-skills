# Skill Benchmark: nvidia-app

> ✅ **Overall verdict: PASS — Recommended for publication**

## Publication Recommendation

Recommended for publication based on the completed evaluation evidence in this report.

## Evaluation Metadata

- Skill: `nvidia-app`
- Evaluation date: 2026-09-28
- Evaluator version: `1.5.6`
- Agents: Claude Code (`aws/anthropic/bedrock-claude-opus-4-8`), Codex (`openai/openai/gpt-5.5`)
- Tasks: 32 evaluation tasks (29 positive, 3 negative)
- Dataset digest: `sha256:24a80b6a8c68db3347169c24fd3020997f52e4a2b1d6de22376feab66226e32f` (skill-evaluator-dataset-snapshot/1)
- Attempts per task: 3
- Environment: `k8s-sandbox`
- Tier 2 evidence: required for publication
- Tier 3 evidence: required for publication

Each task attempt ran in its own isolated sandbox pod.

## What This Report Answers

The three-tier evaluation checks whether the skill:

- is safe to use;
- produces correct answers;
- is discovered and activated when needed;
- helps the agent complete the user's goal and expected workflow; and
- avoids wasted skill and tool usage.

## Results at a Glance

| Measure | Claude Code (Baseline → Skill Uplift) | Codex (Baseline → Skill Uplift) |
|---|---:|---:|
| Overall | 78.8% — baseline ran, but no comparable score was available; uplift unavailable | 68.0% — baseline ran, but no comparable score was available; uplift unavailable |
| Security | 100.0% → 71.9% (-28.1 points) | 81.2% → 76.3% (-4.9 points) |
| Correctness | 9.3% → 86.9% (+77.6 points) | 16.6% → 57.5% (+40.9 points) |
| Discoverability | 97.9% — baseline ran, but no comparable score was available; uplift unavailable | 81.6% — baseline ran, but no comparable score was available; uplift unavailable |
| Effectiveness | 22.2% → 41.1% (+18.9 points) | 22.7% → 31.0% (+8.3 points) |
| Efficiency | 96.1% — baseline ran, but no comparable score was available; uplift unavailable | 93.6% — baseline ran, but no comparable score was available; uplift unavailable |

**How to read this table:** baseline is the same task attempted without the target skill. Scores are rounded to one decimal; threshold-adjacent values use additional precision so their displayed band matches the verdict. Uplift is derived from those displayed scores and shown in percentage points.

Example: `47.0% → 92.0% (+45.0 points)` means the skill-assisted run scored 92.0%, 45.0 percentage points above its 47.0% no-skill baseline.

A partial dimension was calculated from only the available configured signals; review the detailed report before relying on it.

## Token Usage

Actual Tier 3 execution usage is reported for every observed agent/case pair and both conditions.

| Agent | Dataset case | With skill | Without skill | Delta | Change | Coverage |
|---|---|---:|---:|---:|---:|---|
| claude-code | All cases | 6,034,377 | 6,671,615 | N/A | N/A | skill 32/32; base 80/80 |
| claude-code | nvidia-app-applications-list-024 | 233,554 | 395,387 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-compound-010 | 188,012 | 272,534 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-connection-default-012 | 104,063 | 182,201 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-current-game-008 | 189,485 | 88,788 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-driver-discovery-018 | 194,200 | 461,117 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-driver-release-notes-026 | 195,504 | 327,595 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-game-optimization-027 | 241,933 | 593,389 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-game-optimization-battery-031 | 200,455 | 212,120 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-game-optimization-configuration-prerequisite-033 | 110,948 | 123,660 | -12,712 | -10.28% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-game-optimization-default-ac-030 | 198,716 | 398,987 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-game-optimization-discovery-019 | 107,848 | 60,861 | +46,987 | +77.20% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-game-optimization-resolution-prerequisite-032 | 241,386 | 256,455 | -15,069 | -5.88% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-highlights-disable-020 | 237,609 | 242,131 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-highlights-enable-014 | 234,040 | 119,428 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-instant-replay-disable-023 | 230,690 | 89,121 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-instant-replay-enable-003 | 189,234 | 88,518 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-instant-replay-save-005 | 266,589 | 303,368 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-instant-replay-toggle-004 | 230,761 | 240,999 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-laptop-global-read-028 | 197,228 | 179,488 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-laptop-global-set-029 | 197,752 | 120,182 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-launch-025 | 244,873 | 88,493 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-negative-broadcast-016 | 65,626 | 29,914 | +35,712 | +119.38% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-negative-desktop-capture-015 | 65,136 | 125,123 | -59,987 | -47.94% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-negative-obs-017 | 60,414 | 59,981 | +433 | +0.72% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-record-start-001 | 186,892 | 87,864 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-record-stop-002 | 275,340 | 29,724 | +245,616 | +826.32% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-rtx-dvc-enable-021 | 187,577 | 272,610 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-rtx-dvc-toggle-022 | 193,964 | 337,010 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-screenshot-006 | 187,134 | 178,529 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-stats-007 | 189,179 | 276,843 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-status-009 | 296,994 | 369,316 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-unsupported-qualifier-011 | 91,241 | 59,879 | +31,362 | +52.38% | skill 1/1; base 1/1 |
| codex | All cases | 5,670,979 | 8,891,136 | N/A | N/A | skill 40/40; base 77/77 |
| codex | nvidia-app-applications-list-024 | 230,451 | 958,970 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-compound-010 | 127,507 | 481,744 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-connection-default-012 | 47,387 | 51,632 | -4,245 | -8.22% | skill 1/1; base 1/1 |
| codex | nvidia-app-current-game-008 | 196,296 | 485,075 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-driver-discovery-018 | 107,470 | 209,509 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-driver-release-notes-026 | 174,005 | 37,973 | +136,032 | +358.23% | skill 1/1; base 1/1 |
| codex | nvidia-app-game-optimization-027 | 649,355 | 1,896,371 | -1,247,016 | -65.76% | skill 3/3; base 3/3 |
| codex | nvidia-app-game-optimization-battery-031 | 319,437 | 1,278,449 | N/A | N/A | skill 2/2; base 3/3 |
| codex | nvidia-app-game-optimization-configuration-prerequisite-033 | 111,285 | 77,806 | +33,479 | +43.03% | skill 1/1; base 1/1 |
| codex | nvidia-app-game-optimization-default-ac-030 | 126,245 | 885,724 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-game-optimization-discovery-019 | 87,707 | 32,299 | +55,408 | +171.55% | skill 1/1; base 1/1 |
| codex | nvidia-app-game-optimization-resolution-prerequisite-032 | 129,126 | 14,009 | +115,117 | +821.74% | skill 1/1; base 1/1 |
| codex | nvidia-app-highlights-disable-020 | 251,506 | 297,247 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-highlights-enable-014 | 167,711 | 211,779 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-instant-replay-disable-023 | 232,715 | 68,814 | N/A | N/A | skill 2/2; base 3/3 |
| codex | nvidia-app-instant-replay-enable-003 | 251,961 | 40,703 | N/A | N/A | skill 2/2; base 3/3 |
| codex | nvidia-app-instant-replay-save-005 | 147,099 | 112,001 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-instant-replay-toggle-004 | 106,940 | 109,316 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-laptop-global-read-028 | 580,408 | 168,690 | N/A | N/A | skill 2/2; base 3/3 |
| codex | nvidia-app-laptop-global-set-029 | 87,243 | 144,208 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-launch-025 | 107,745 | 95,469 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-negative-broadcast-016 | 33,855 | 31,845 | +2,010 | +6.31% | skill 1/1; base 1/1 |
| codex | nvidia-app-negative-desktop-capture-015 | 34,578 | 32,379 | +2,199 | +6.79% | skill 1/1; base 1/1 |
| codex | nvidia-app-negative-obs-017 | 147,374 | 128,267 | +19,107 | +14.90% | skill 1/1; base 1/1 |
| codex | nvidia-app-record-start-001 | 146,024 | 68,063 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-record-stop-002 | 125,975 | 54,848 | N/A | N/A | skill 1/1; base 2/2 |
| codex | nvidia-app-rtx-dvc-enable-021 | 180,447 | 102,285 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-rtx-dvc-toggle-022 | 132,328 | 109,410 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-screenshot-006 | 169,881 | 245,520 | -75,639 | -30.81% | skill 3/3; base 3/3 |
| codex | nvidia-app-stats-007 | 142,497 | 109,516 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-status-009 | 275,751 | 309,215 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-unsupported-qualifier-011 | 42,670 | 42,000 | +670 | +1.60% | skill 1/1; base 1/1 |
| ALL AGENTS | Dataset aggregate | 11,705,356 | 15,562,751 | N/A | N/A | skill 72/72; base 157/157 |

Prompt tokens include cached reads, so total tokens are `prompt + completion` (cached is not added twice). The Efficiency score uses `(prompt - cached) + completion`. N/A means the relevant trajectory counters were not available; coverage is never estimated.

## Tier Status

| Tier | Purpose | Status | Evidence |
|---|---|---|---|
| Tier 1 | Static validation | **PASSED WITH OBSERVATIONS** | 11 validator(s); 3 finding(s) |
| Tier 2 | Semantic deduplication | **PASSED** | 2 validator(s); 0 finding(s) |
| Tier 3 | Live agent evaluation | **PASS** | 2 agent(s); 32 task(s) |

## Findings and Observations

<details>
<summary>Show detailed findings and successful checks</summary>

- **MEDIUM** QUALITY/quality_efficiency: Deeply nested references in overlay-state.md (`skills/nvidia-app/SKILL.md`)
- **LOW** QUALITY/quality_discoverability: Description doesn't mention WHEN to use this skill (`skills/nvidia-app/SKILL.md`)
- **LOW** QUALITY/quality_discoverability: Broad description without negative triggers may cause over-triggering (`skills/nvidia-app/SKILL.md`)

</details>

## Scoring Methodology

<details>
<summary>Show dimension definitions, source signals, and thresholds</summary>

| Dimension | Question | Scored signals |
|---|---|---|
| Security | Is it safe to use? | `security` (100%) |
| Correctness | Is the answer correct? | `accuracy` (100%) |
| Discoverability | Was the right skill loaded when needed? | `skill_execution` (100%) |
| Effectiveness | Did the skill help complete the task? | `goal_accuracy` (50%) + `behavior_check` (50%) |
| Efficiency | Did it avoid wasted tool calls and token usage? | `skill_efficiency` (50%) + `token_efficiency` (50%) |

- Dimension bands: PASS at 50% or above; NEUTRAL from 40% to below 50%; FAIL below 40%.
- Overall Tier 3 lift: PASS at +5 points or more; FAIL at -10 points or less; values between those bands are NEUTRAL.
- Overall verdict: PASS only when every configured dimension passes for at least one supported agent. Lift is reported as diagnostic evidence and does not override this gate.
- The 50% attempt pass threshold is a separate per-task gate; it is not the dimension pass threshold.
- Effectiveness is the equal-weight mean of goal completion (`goal_accuracy`) and expected workflow adherence (`behavior_check`).
- Efficiency is 50% tool-call productivity (the backward-compatible `skill_efficiency` wire id) and 50% `token_efficiency`. Positive-case skill routing is scored under Discoverability, not Efficiency; a negative case without a routing target is N/A. N/A sources are omitted, remaining weights are renormalized, and the dimension is marked partial.

Signals present in this run:

- `security` (Security): unsafe operations, secret leakage, and unauthorized access.
- `skill_execution` (Skill Execution): whether the expected skill was selected, decoys were avoided, and the workflow executed.
- `skill_efficiency` (Tool Productivity): tool-call productivity (legacy wire id; routing is scored under Discoverability).
- `accuracy` (Accuracy): final-answer correctness against the reference answer.
- `goal_accuracy` (Goal Accuracy): whether the user's goal was achieved.
- `behavior_check` (Behavior Check): whether the expected workflow behavior was followed.
- `token_efficiency` (Token Efficiency): actual uncached prompt plus completion usage (50% of Efficiency).

</details>

## Freshness

Regenerate this benchmark when the skill, evaluation dataset, target agent/model, evaluator version, environment, or scoring policy changes.
