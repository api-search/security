---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods described across the provided pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Codekeeperbv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codekeeperbv declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Codekeeperbv
provider_slug: codekeeperbv
scheme_count: 2
schemes:
- evidence: Cybercriminals exploit OAuth device codes to hack Microsoft 365 accounts
  name: OAuth device code flow
  type: oauth2
- evidence: authentication bypass is more severe, letting attackers gain admin access by sending Basic auth headers
  header: Authorization
  location: header
  name: Basic Authentication
  type: http-basic
slug: codekeeperbv-authentication
source_filename: codekeeperbv-authentication.yml
source_heading: Authentication Profile
source_url: https://codekeeper.co/hubfs/Markdown/ticker-cybercriminals-abuse-oauth-device-codes-in-microsoft-365-attacks.md
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://codekeeper.co/hubfs/Markdown/ticker-cybercriminals-abuse-oauth-device-codes-in-microsoft-365-attacks.md\nsources:\n- https://codekeeper.co/hubfs/Markdown/ticker-cybercriminals-abuse-oauth-device-codes-in-microsoft-365-attacks.md\n- https://codekeeper.co/hubfs/Markdown/ticker-gitlab-security-updates-critical-vulnerabilities.md\n- https://codekeeper.co/hubfs/Markdown/ticker-linux-cups-vulnerabilities-disrupt-print-authentication.md\n- https://codekeeper.co/hubfs/Markdown/ticker-phishing-attack-targets-35000-users-with-mfa-bypass.md\ndescription: Authentication methods described across the provided pages.\nschemes:\n- type: oauth2\n  name: OAuth device code flow\n  evidence: Cybercriminals exploit OAuth device codes to hack Microsoft 365 accounts\n- type: http-basic\n  name: Basic Authentication\n  evidence: authentication bypass is more severe, letting attackers gain admin\
  \ access by sending Basic auth headers\n  location: header\n  header: Authorization\ndocs: https://codekeeper.co/hubfs/Markdown/ticker-cybercriminals-abuse-oauth-device-codes-in-microsoft-365-attacks.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codekeeperbv/refs/heads/main/authentication/codekeeperbv-authentication.yml
summary_line: 2 schemes
tags:
- Software Escrow
- Continuity
- SaaS
- Backup
- AI
- Compliance
- Vendor Risk
---
