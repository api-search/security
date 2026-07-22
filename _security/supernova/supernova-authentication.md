---
api_key_in:
- token
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Supernova Authentication
name_suffix: Authentication
oauth_flows: []
overview: Supernova secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Supernova
provider_slug: supernova
scheme_count: 1
schemes:
- name: PersonalAccessToken
  obtained_from: Supernova.io account / workspace settings
  scheme: token
  sources:
  - https://registry.npmjs.org/@supernovaio/sdk
  type: apiKey
  used_by:
  - '@supernovaio/sdk'
  - '@supernovaio/cli'
slug: supernova-authentication
source_filename: supernova-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://registry.npmjs.org/@supernovaio/sdk (SDK readme — \"Obtaining API Key\")\ndocs: https://developers.supernova.io/\nsummary:\n  types: [apiKey]\n  api_key_in: [token]\n  oauth2_flows: []\n  note: >-\n    Supernova exposes no public REST OpenAPI; programmatic access is via the official\n    JS/TS SDK and CLI. Both authenticate with a personal access key (API token) obtained\n    from the Supernova.io account settings. Enterprise workspaces additionally support\n    SSO and SCIM provisioning for platform (human) access.\nschemes:\n  - name: PersonalAccessToken\n    type: apiKey\n    scheme: token\n    obtained_from: Supernova.io account / workspace settings\n    used_by:\n      - \"@supernovaio/sdk\"\n      - \"@supernovaio/cli\"\n    sources:\n      - https://registry.npmjs.org/@supernovaio/sdk\nenterprise_identity:\n  sso: true\n  scim: true\n  source: https://learn.supernova.io/changelog (June 2026 — SCIM provisioning)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supernova/refs/heads/main/authentication/supernova-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Design Tech
- Design Systems
- Design Tokens
- Documentation
- Code Automation
- Developer Experience
- AI Agents
- MCP
---
