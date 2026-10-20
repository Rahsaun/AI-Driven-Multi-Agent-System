# Experiment Log

This page preserves the chronological records from the original README. Some observations are described at a high level because detailed command/output transcripts have not yet been included.

## April 23, 2026 — Project initialized

- Created the GitHub repository to document findings.
- Defined initial research questions.
- Began researching AI-agent behavior on live systems.

## May 16, 2026 — Virtual machine setup

- Installed and configured the virtual machine.
- Selected a guest OS and configured networking.
- Took a baseline snapshot before AI interaction.

## May 23, 2026 — First AI session

- Gave Claude initial instructions in the VM.
- Observed file-system exploration and terminal command usage.
- Reported logging commands and responses.
- Collaborated with Claude to write an email script stored on Ubuntu and launched from the terminal.
- The script used stored Gmail credentials and requested a recipient, subject, and message body.
- A test email was sent successfully, including an automatic “Best regards” sign-off.

**Interpretation:** This demonstrates a human-assisted workflow where AI authored a script that a human then ran. It does not, by itself, demonstrate fully autonomous email composition or delivery.

## May 23, 2026 — Security testing begins

- Began studying file modification, process creation, and possible permission escalation behavior.
- Started recording unexpected actions and access patterns.

The original README does not provide detailed results for each security scenario.

## May 24, 2026 — API research

- Investigated connecting to Claude's API to support more autonomous email-related tasks.
- Noted API billing through an Anthropic account.
- Documented a proposed initial experiment budget of $10 in API credits; this was a plan, not a confirmed expense.

## Future experiment entry template

### YYYY-MM-DD — Experiment name

- **Objective:**
- **VM snapshot / configuration:**
- **AI model and permissions:**
- **Input / task:**
- **Observed behavior:**
- **Evidence / log location:**
- **Outcome:**
- **Security implications:**

Related: [Environment](environment.md) · [Security Findings](security.md).
