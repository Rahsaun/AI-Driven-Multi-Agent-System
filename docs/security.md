# Security Findings and Anomalies

This page separates observed events from possible risks. A theoretical capability is not proof that an exploit occurred.

## Observations

### Outbound network access

A script operating inside the Ubuntu VM successfully sent an email using SMTP. This confirms an outbound communication path existed at the time of the test.

**Potential risk:** If an agent had inappropriate access to sensitive data and the same network path, unauthorized data transfer could be possible. No such transfer is demonstrated by the existing notes.

### Unexpected recipient behavior

The original email script initially defaulted to a recipient instead of requesting a new one, and an email was sent to the wrong recipient. Later revisions prompted for the recipient and subject.

**Lesson:** Outbound actions should display their intended target and require explicit user confirmation.

## Recorded errors

| Date | Incident | Documented response |
|---|---|---|
| May 22, 2026 | Could not access the Gmail account | Original log reports an error and subsequent resolution by granting access to a Google API key |
| May 22, 2026 | Email script sent to an unintended default recipient | Revised the script to prompt for recipient and subject |

## Recommended controls for upcoming experiments

- Require explicit approval before sending messages or modifying important files.
- Allowlist tools, file paths, and network destinations as appropriate.
- Store secrets outside source code and redact them from logs.
- Record timestamps, commands, outputs, and approval decisions.
- Use dedicated test credentials and synthetic data.
- Verify VM networking settings rather than assuming complete isolation.

## Unresolved questions

- What exact permissions did the AI receive in each test?
- Which actions were chosen by AI versus executed manually?
- Were network and file-access controls enforced?
- What happened during the reported permission-escalation testing?

See [Experiments](experiments.md) for the research chronology.
