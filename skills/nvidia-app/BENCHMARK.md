# Skill Benchmark: nvidia-app

> ✅ **Overall verdict: PASS — Recommended for publication**

## Publication Recommendation

Recommended for publication based on the completed evaluation evidence in this report.

## Evaluation Metadata

- Skill: `nvidia-app`
- Evaluation date: 2026-09-17
- Evaluator version: `1.5.6`
- Agents: Claude Code (`aws/anthropic/bedrock-claude-opus-4-8`), Codex (`openai/openai/gpt-5.5`)
- Tasks: 28 evaluation tasks (25 positive, 3 negative)
- Dataset digest: `sha256:59e6c0aba7b851bb7a8a6bb645dd1c63f94c31e06ee0cea45fa5e1c84a2aab52` (skill-evaluator-dataset-snapshot/1)
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
| Overall | 79.3% — baseline ran, but no comparable score was available; uplift unavailable | 67.9% — baseline ran, but no comparable score was available; uplift unavailable |
| Security | 100.0% → 76.8% (-23.2 points) | 84.0% → 74.2% (-9.8 points) |
| Correctness | 8.7% → 85.0% (+76.3 points) | 15.0% → 56.4% (+41.4 points) |
| Discoverability | 97.6% — baseline ran, but no comparable score was available; uplift unavailable | 83.7% — baseline ran, but no comparable score was available; uplift unavailable |
| Effectiveness | 20.3% → 40.7% (+20.4 points) | 22.0% → 30.9% (+8.9 points) |
| Efficiency | 96.3% — baseline ran, but no comparable score was available; uplift unavailable | 94.4% — baseline ran, but no comparable score was available; uplift unavailable |

**How to read this table:** baseline is the same task attempted without the target skill. Scores are rounded to one decimal; threshold-adjacent values use additional precision so their displayed band matches the verdict. Uplift is derived from those displayed scores and shown in percentage points.

Example: `47.0% → 92.0% (+45.0 points)` means the skill-assisted run scored 92.0%, 45.0 percentage points above its 47.0% no-skill baseline.

A partial dimension was calculated from only the available configured signals; review the detailed report before relying on it.

## Token Usage

Actual Tier 3 execution usage is reported for every observed agent/case pair and both conditions.

| Agent | Dataset case | With skill | Without skill | Delta | Change | Coverage |
|---|---|---:|---:|---:|---:|---|
| claude-code | All cases | 4,813,340 | 5,541,925 | N/A | N/A | skill 28/28; base 76/76 |
| claude-code | nvidia-app-applications-list-024 | 192,995 | 366,888 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-compound-010 | 189,851 | 242,590 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-connection-default-012 | 104,025 | 89,593 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-current-game-008 | 188,394 | 88,169 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-driver-discovery-018 | 196,036 | 455,457 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-driver-release-notes-026 | 195,328 | 358,539 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-game-optimization-027 | 197,356 | 459,935 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-game-optimization-discovery-019 | 106,683 | 90,149 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-highlights-disable-020 | 188,478 | 180,383 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-highlights-enable-014 | 151,126 | 149,942 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-instant-replay-disable-023 | 229,977 | 89,081 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-instant-replay-enable-003 | 195,713 | 89,282 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-instant-replay-save-005 | 187,371 | 273,129 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-instant-replay-toggle-004 | 187,956 | 333,646 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-laptop-global-read-028 | 193,279 | 119,972 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-laptop-global-set-029 | 235,241 | 212,228 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-launch-025 | 196,407 | 88,380 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-negative-broadcast-016 | 65,910 | 29,944 | +35,966 | +120.11% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-negative-desktop-capture-015 | 65,201 | 60,940 | +4,261 | +6.99% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-negative-obs-017 | 61,030 | 92,024 | -30,994 | -33.68% | skill 1/1; base 1/1 |
| claude-code | nvidia-app-record-start-001 | 145,479 | 87,864 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-record-stop-002 | 186,272 | 89,175 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-rtx-dvc-enable-021 | 226,625 | 212,944 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-rtx-dvc-toggle-022 | 191,124 | 373,703 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-screenshot-006 | 146,892 | 208,640 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-stats-007 | 231,285 | 303,766 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-status-009 | 296,707 | 335,648 | N/A | N/A | skill 1/1; base 3/3 |
| claude-code | nvidia-app-unsupported-qualifier-011 | 60,599 | 59,914 | +685 | +1.14% | skill 1/1; base 1/1 |
| codex | All cases | 4,649,503 | 6,759,406 | N/A | N/A | skill 33/33; base 72/72 |
| codex | nvidia-app-applications-list-024 | 127,163 | 804,748 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-compound-010 | 131,482 | 266,914 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-connection-default-012 | 47,421 | 107,945 | -60,524 | -56.07% | skill 1/1; base 1/1 |
| codex | nvidia-app-current-game-008 | 250,747 | 279,127 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-driver-discovery-018 | 127,246 | 207,129 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-driver-release-notes-026 | 146,876 | 184,172 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-game-optimization-027 | 823,820 | 2,307,693 | N/A | N/A | skill 2/2; base 3/3 |
| codex | nvidia-app-game-optimization-discovery-019 | 48,651 | 78,162 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-highlights-disable-020 | 153,585 | 271,226 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-highlights-enable-014 | 105,601 | 254,925 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-instant-replay-disable-023 | 86,276 | 49,290 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-instant-replay-enable-003 | 125,438 | 68,421 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-instant-replay-save-005 | 129,465 | 152,677 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-instant-replay-toggle-004 | 126,124 | 100,866 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-laptop-global-read-028 | 107,495 | 124,717 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-laptop-global-set-029 | 392,756 | 153,372 | N/A | N/A | skill 2/2; base 3/3 |
| codex | nvidia-app-launch-025 | 107,317 | 96,249 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-negative-broadcast-016 | 55,122 | 18,001 | +37,121 | +206.22% | skill 1/1; base 1/1 |
| codex | nvidia-app-negative-desktop-capture-015 | 29,737 | 34,966 | -5,229 | -14.95% | skill 1/1; base 1/1 |
| codex | nvidia-app-negative-obs-017 | 119,387 | 108,436 | +10,951 | +10.10% | skill 1/1; base 1/1 |
| codex | nvidia-app-record-start-001 | 167,247 | 91,596 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-record-stop-002 | 307,553 | 115,031 | N/A | N/A | skill 2/2; base 3/3 |
| codex | nvidia-app-rtx-dvc-enable-021 | 163,465 | 111,581 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-rtx-dvc-toggle-022 | 123,506 | 99,295 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-screenshot-006 | 300,747 | 217,423 | +83,324 | +38.32% | skill 3/3; base 3/3 |
| codex | nvidia-app-stats-007 | 105,081 | 27,213 | +77,868 | +286.14% | skill 1/1; base 1/1 |
| codex | nvidia-app-status-009 | 160,490 | 371,120 | N/A | N/A | skill 1/1; base 3/3 |
| codex | nvidia-app-unsupported-qualifier-011 | 79,705 | 57,111 | +22,594 | +39.56% | skill 1/1; base 1/1 |
| ALL AGENTS | Dataset aggregate | 9,462,843 | 12,301,331 | N/A | N/A | skill 61/61; base 148/148 |

Prompt tokens include cached reads, so total tokens are `prompt + completion` (cached is not added twice). The Efficiency score uses `(prompt - cached) + completion`. N/A means the relevant trajectory counters were not available; coverage is never estimated.

## Tier Status

| Tier | Purpose | Status | Evidence |
|---|---|---|---|
| Tier 1 | Static validation | **PASSED WITH OBSERVATIONS** | 11 validator(s); 1 finding(s) |
| Tier 2 | Semantic deduplication | **PASSED** | 2 validator(s); 0 finding(s) |
| Tier 3 | Live agent evaluation | **PASS** | 2 agent(s); 28 task(s) |

## Findings and Observations

<details>
<summary>Show detailed findings and successful checks</summary>

- **MEDIUM** QUALITY/quality_efficiency: Deeply nested references in overlay-state.md (`skills/nvidia-app/SKILL.md`)

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
