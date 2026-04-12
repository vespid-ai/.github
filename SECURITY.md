# Security Policy

This organization publishes early open-source infrastructure for trustworthy agent execution: runtime control, delegated authorization, operator portability, and related public documentation.

## Supported status

The repositories under `vespid-ai` are active public work, but they should be treated as evolving infrastructure rather than hardened production systems by default.

Some repos publish more specific `SECURITY.md` files. When a repository has its own security policy, that repo-specific policy takes precedence over this organization default.

## Reporting a vulnerability

Please do not open a public issue for a sensitive security report.

Use one of these paths instead:

- GitHub private vulnerability reporting / security advisory flow, if enabled for the affected repository
- private contact with the repository or organization owner via GitHub

Please include:

- the affected repository, command, service, or integration surface
- reproduction steps
- the likely security impact
- whether secrets, approval boundaries, delegated authorization, or protected actions are involved

## Highest-priority reports

We care most about reports involving:

- credential, token, cookie, or secret leakage
- approval or protected-action bypasses
- sandbox escape, path traversal, or unsafe filesystem access
- delegated-capability scope escalation or trust-boundary confusion
- operator-state export/import bugs that expose sensitive data
- unsafe defaults that could make irreversible actions easier than intended

## Expectations

These projects aim to make agent systems more inspectable and controllable. That does not mean every repository is a complete security boundary on its own. Review the trust model of each repository before using it in sensitive production workflows.
