## Description: <br>
Use NVIDIA App's local MCP tools for application, driver, game-optimization, laptop-feature, and restricted In-Game Overlay operations and troubleshooting. <br>

This skill is ready for commercial/non-commercial use. <br>

## Owner
NVIDIA <br>

### License/Terms of Use: <br>
CC-BY-4.0 AND Apache 2.0 <br>
## Use Case: <br>
Developers and engineers who use NVIDIA App to manage drivers, optimize game settings, and control In-Game Overlay recording, screenshots, and display features through local MCP tools. <br>

### Deployment Geography for Use: <br>
Global <br>

## Requirements / Dependencies: <br>
**Requires API Key or External Credential:** [Yes] <br>
**Credential Type(s):** [API key] <br>

Do not include secrets in prompts/logs/output; use least-privilege credentials; rotate keys as appropriate. <br>

## Known Risks and Mitigations: <br>
Risk: Review before execution as proposals could introduce incorrect or misleading guidance into skills. <br>
Mitigation: Review and scan skill before deployment. <br>

## Reference(s): <br>
- [connection.md](references/connection.md) <br>
- [general-tools.md](references/general-tools.md) <br>
- [mcp-tool-contract.md](references/mcp-tool-contract.md) <br>
- [overlay-capture.md](references/overlay-capture.md) <br>
- [overlay-state.md](references/overlay-state.md) <br>


## Skill Output: <br>
**Output Type(s):** [API Calls, Analysis, Configuration instructions] <br>
**Output Format:** [Markdown with inline JSON code blocks] <br>
**Output Parameters:** [1D] <br>
**Other Properties Related to Output:** [None] <br>

## Evaluation Agents Used: <br>
- Claude Code (`aws/anthropic/bedrock-claude-opus-4-8`) <br>
- Codex (`openai/openai/gpt-5.5`) <br>



## Evaluation Tasks: <br>
28 evaluation tasks (25 positive, 3 negative), each run with 3 attempts per task in isolated k8s-sandbox pods. <br>

## Evaluation Metrics Used: <br>
Reported benchmark dimensions: <br>
- Security: Checks for unsafe operations, secret leakage, and unauthorized access. <br>
- Correctness: Checks final-answer correctness against the reference answer. <br>
- Discoverability: Checks whether the expected skill was selected and the workflow executed. <br>
- Effectiveness: Checks whether the user's goal was achieved and the expected workflow behavior was followed (50% goal_accuracy + 50% behavior_check). <br>
- Efficiency: Checks tool-call productivity and token efficiency (50% skill_efficiency + 50% token_efficiency). <br>

Underlying evaluation signals used in this run: <br>
- `security`: Detects unsafe operations, secret leakage, and unauthorized access. <br>
- `accuracy`: Verifies final-answer correctness against the reference answer. <br>
- `skill_execution`: Verifies the expected skill was selected, decoys were avoided, and the workflow executed. <br>
- `goal_accuracy`: Verifies whether the user's goal was achieved. <br>
- `behavior_check`: Verifies whether the expected workflow behavior was followed. <br>
- `skill_efficiency`: Measures tool-call productivity. <br>
- `token_efficiency`: Measures actual uncached prompt plus completion token usage. <br>



## Evaluation Results: <br>
| Measure | Claude Code (Baseline → Skill Uplift) | Codex (Baseline → Skill Uplift) |
|---|---:|---:|
| Overall | 79.3% — baseline ran, but no comparable score was available; uplift unavailable | 67.9% — baseline ran, but no comparable score was available; uplift unavailable |
| Security | 100.0% → 76.8% (-23.2 points) | 84.0% → 74.2% (-9.8 points) |
| Correctness | 8.7% → 85.0% (+76.3 points) | 15.0% → 56.4% (+41.4 points) |
| Discoverability | 97.6% — baseline ran, but no comparable score was available; uplift unavailable | 83.7% — baseline ran, but no comparable score was available; uplift unavailable |
| Effectiveness | 20.3% → 40.7% (+20.4 points) | 22.0% → 30.9% (+8.9 points) |
| Efficiency | 96.3% — baseline ran, but no comparable score was available; uplift unavailable | 94.4% — baseline ran, but no comparable score was available; uplift unavailable |

## Skill Version(s): <br>
1.1.5 (source: frontmatter) <br>

## Ethical Considerations: <br>
NVIDIA believes Trustworthy AI is a shared responsibility and we have established policies and practices to enable development for a wide array of AI applications. When downloaded or used in accordance with our terms of service, developers should work with their internal team to ensure this skill meets requirements for the relevant industry and use case and addresses unforeseen product misuse. <br>

(For Release on NVIDIA Platforms Only) <br>
Please report quality, risk, security vulnerabilities or NVIDIA AI Concerns [here](https://app.intigriti.com/programs/nvidia/nvidiavdp/detail). <br>
