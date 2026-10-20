# Setup and Environment

This page records the environment described in the original project README. It is a research record, not a fully reproducible setup guide.

| Component | Documented configuration |
|---|---|
| Virtualization platform | VirtualBox |
| Host operating system | Windows 11 Home |
| Guest operating system | Ubuntu 22.04 |
| AI | Claude (listed as Claude Sonnet 4.6 in original notes) |
| Interface | Terminal and API-based workflows |
| Logging | Manual logs and GitHub documentation |
| Snapshot strategy | Baseline snapshot and snapshots after major milestones |

## Network configuration

The original log describes the VM networking as **NAT / bridged** and reports successful outbound email delivery using SMTP.

**Important:** NAT and bridged networking are not equivalent to an air-gapped or fully isolated VM. Outbound email delivery confirms that network communication was possible. Treat any claim of total isolation as unverified.

## Precautions for future experiments

- Use synthetic test data and non-sensitive test accounts.
- Keep permissions narrowly scoped and require human approval before consequential actions.
- Avoid mounting sensitive host folders or exposing personal credentials inside the VM.
- Document the exact network mode, snapshot identifier, model, and tool permissions for each experiment.
- Do not commit API keys, passwords, or credential files.

See [Security Findings](security.md) for the known observations.
