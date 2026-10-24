# Security policy

## Report a vulnerability privately

Email [apedinfamily@outlook.com](mailto:apedinfamily@outlook.com) with the subject **apedin security report**.

Please do not put vulnerability details, account data or exploit demonstrations in public issues, discussions or social posts. GitHub private vulnerability reporting is not required to use this email channel.

Include, where possible:

- The affected page or feature and when you observed the issue.
- Clear reproduction steps using an account or data you control.
- The expected behaviour, actual behaviour and potential impact.
- Minimal supporting evidence with sensitive values removed.
- A way to contact you for clarification.

Do not send passwords, recovery phrases, private keys, session tokens or other people's personal data. If sensitive information was exposed, describe its type and location without including its contents.

## Scope

This policy covers suspected vulnerabilities affecting the current apedin service at [apedin.family](https://apedin.family/) and material published in this public documentation repository. The application source is private; a report does not require source access.

Relevant issues include unauthorised account access, cross-account changes, private-data exposure, script injection, improper profile ownership claims, and manipulation of account or progression records across a trust boundary.

Independent providers, wallets and linked websites are operated by their respective owners. Report vulnerabilities confined to those services through their own channels. If an apedin integration exposes apedin users, please tell us about that impact too.

## Important security boundaries

- Publicly imported profiles and activity must not by themselves grant account access or ownership.
- Account changes must be authorised for the affected account; signing in must not silently merge unrelated identities.
- Untrusted posts, profile fields, links and uploaded media must not become executable application content.
- Operator-only ingestion and moderation functions must not be available to ordinary visitors.

These describe properties the service should preserve, not a guarantee that every implementation path is free of defects.

## Research and disclosure

Use your own accounts and the minimum interaction needed to demonstrate an issue. Do not access other people's data, disrupt availability, run high-volume scans, send phishing messages or test third-party systems without their permission. If you encounter another person's information, stop and report the location privately.

We assess reports based on reproducibility and impact, and coordinate appropriate fixes and disclosure. Please keep details private while we investigate and agree a disclosure plan with you. There is no guaranteed response or remediation deadline, and this policy does not establish a paid bug-bounty programme or grant blanket testing authorisation.

## Supported service and assessment limits

Security reports should concern the currently hosted service or a risk still present in it. Historical release notes are not a promise to support older deployments or provide self-hosted builds.

Automated scans and internal engineering reviews provide limited evidence. They do not establish that the service is vulnerability-free. See [Transparency](TRANSPARENCY.md#security-review-evidence) for the scope and age of the review information published here.
