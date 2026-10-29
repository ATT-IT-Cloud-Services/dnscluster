# Security Policy

## Supported versions

| Version | Supported |
| --- | --- |
| 1.x | ✅ |
| < 1.0 | ❌ |

Security fixes are applied to the latest 1.x release line.

## Reporting a vulnerability

Please report suspected vulnerabilities **privately** to
[service@att-it.com](mailto:service@att-it.com).

Include:

- the affected repository and version/commit,
- a description of the issue and its impact,
- reproduction steps or a proof of concept,
- any suggested remediation.

Please do **not** open a public GitHub issue for an undisclosed
vulnerability. We aim to acknowledge reports within three business days and
will coordinate disclosure after a fix is available.

## Scope

DNS cluster configuration, PowerDNS APIs, TSIG/authentication secrets, database access and network exposure of DNS services.

Review `docker-compose.yml`, firewall rules and secret files before exposing DNS or PowerDNS-Admin publicly.

## General expectations

- Never commit API keys, passwords, tokens, private keys or production
  credentials. Use environment variables or the deployment secret store.
- Keep dependencies and base images up to date.
- Treat all user-controlled input, template data, repository content and
  webhook payloads as untrusted.
- Do not test against systems or data you do not own or have permission to
  test.

## Safe harbour

Good-faith security research that respects this policy, avoids privacy
violations, data destruction and service disruption, and gives us reasonable
time to remediate will not be pursued by us.

© ATT IT / Philippe Simon Pflug. All rights reserved.
