# AI-Driven Multi-Agent System

A personal research project exploring **AI behavior, autonomy, reliability, and security** when AI tools interact with an operating system inside a virtual machine.

## Project goal

Study what AI systems do when given operating-system tools, document unexpected behavior, and develop safer approaches to agentic computing. The long-term direction is to explore collaboration among multiple AI agents.

> **Project status:** Experimental research and documentation. The current records describe Claude-assisted terminal and email scripting experiments; a functioning multi-agent system has not yet been documented.

## Documentation

| Start here | What you will find |
|---|---|
| [Project overview](docs/overview.md) | Motivation, goals, scope, and research questions |
| [Environment and setup](docs/environment.md) | VirtualBox, Ubuntu, AI interface, network configuration, and precautions |
| [Experiment log](docs/experiments.md) | Dated sessions and observed results |
| [Security findings](docs/security.md) | Observations, anomalies, potential risks, and mitigations |
| [Project roadmap](docs/roadmap.md) | Upcoming agent, security, and research milestones |

## Research environment

- **Host OS:** Windows 11 Home
- **Virtualization:** VirtualBox
- **Guest OS:** Ubuntu 22.04
- **AI:** Claude
- **Interaction methods:** Terminal scripts and API research

See [Environment and setup](docs/environment.md) for the recorded configuration and its limitations.

## Highlights so far

- Set up and documented a virtual-machine research environment.
- Used Claude to help write a terminal-executed email script.
- Sent a test email using that script, then improved recipient prompts after an error.
- Identified outbound network connectivity as a security consideration.

For precise dates, outcomes, and qualifications, read the [Experiment log](docs/experiments.md).

## Next steps

Develop agent roles, introduce structured logging and human approval controls, broaden experiments, and compare models. Track progress on the [Roadmap](docs/roadmap.md).

## Research and safety

The project is intended for controlled, educational experimentation. VM networking may allow external connectivity; virtual machines are not automatically fully isolated. Use synthetic data, dedicated test accounts, least-privilege access, and explicit approval for consequential actions. Do not put passwords or API credentials in repository files.

---

*Documentation reorganized October 20, 2026. Original experiment history is preserved in the linked documents.*
