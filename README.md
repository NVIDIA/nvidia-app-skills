# NVIDIA App Skills

This repository contains an agent skill for operating NVIDIA App through its local Model Context Protocol (MCP) server. The skill supports NVIDIA App queries and actions for applications, drivers, game optimization, laptop features, and selected In-Game Overlay workflows.

## Requirements

- A Windows system with a supported NVIDIA GPU.
- [NVIDIA App](https://www.nvidia.com/en-us/software/nvidia-app/) installed (version 11.0.9.5xx or above).
- MCP server access enabled in NVIDIA App.
- An MCP client that supports Streamable HTTP over loopback or can use the NVIDIA App stdio bridge.
- For In-Game Overlay operations, NVIDIA In-Game Overlay must also be enabled, running, and ready.

## Usage

Ask your agent to perform a supported NVIDIA App task. For example:

- "Show my NVIDIA driver status."
- "List the games and applications detected by NVIDIA App."
- "Optimize the graphics settings for Cyberpunk 2077."
- "Start recording my gameplay."
- "Save my Instant Replay."
- "Show the Statistics Overlay."
- "Enable RTX Dynamic Vibrance."

See the [NVIDIA App skill instructions](skills/nvidia-app/SKILL.md) for the supported workflows, connection behavior, privacy considerations, and troubleshooting guidance.

## Support and contributions

To report a bug, request an enhancement, or ask a project-related question, [file an issue](https://github.com/NVIDIA/nvidia-app-skills/issues).

See [CONTRIBUTING.md](CONTRIBUTING.md) for contribution guidelines. Do not report security vulnerabilities through public GitHub issues; follow the instructions in [SECURITY.md](SECURITY.md) instead.

## References

- [NVIDIA App](https://www.nvidia.com/en-us/software/nvidia-app/)

## License

See [LICENSE](LICENSE) for details.
