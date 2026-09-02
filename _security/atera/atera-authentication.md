---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Atera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atera secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Atera
provider_slug: atera
scheme_count: 1
schemes:
- description: Account-scoped API token supplied on every request. Created in the Atera console under Admin > Data management > API; the token value is shown once at creation and cannot be retrieved afterwards.
  evidence: Atera's own PowerShell sample sets $headers.Add("X-API-KEY", 'YOUR_API_KEY_HERE') and calls https://app.atera.com/api/v3/agents/machine/$ENV:COMPUTERNAME.
  in: header
  name: X-API-KEY
  parameter_name: X-API-KEY
  sources:
  - https://support.atera.com/hc/en-us/articles/219083397-Using-the-Atera-API
  - https://support.atera.com/hc/en-us/articles/115015347567-Script-for-checking-USB-connection-to-devices
  type: apiKey
slug: atera-authentication
source_filename: atera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://support.atera.com/hc/en-us/articles/219083397-Using-the-Atera-API\ndocs: https://support.atera.com/hc/en-us/articles/219083397-Using-the-Atera-API\nnotes: >-\n  Derived by reading Atera's own support documentation, not from an OpenAPI file.\n  Atera states in its API FAQ that the API is driven by OpenAPI 3.0, but the\n  interactive reference at https://app.atera.com/apidocs returns 401 with an empty\n  body to any unauthenticated client, and no specification is published at a public\n  URL, so no securitySchemes could be parsed.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  transport: https-only\nschemes:\n- name: X-API-KEY\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  description: >-\n    Account-scoped API token supplied on every request. Created in the Atera console\n    under Admin > Data management > API;\
  \ the token value is shown once at creation and\n    cannot be retrieved afterwards.\n  sources:\n  - https://support.atera.com/hc/en-us/articles/219083397-Using-the-Atera-API\n  - https://support.atera.com/hc/en-us/articles/115015347567-Script-for-checking-USB-connection-to-devices\n  evidence: >-\n    Atera's own PowerShell sample sets $headers.Add(\"X-API-KEY\", 'YOUR_API_KEY_HERE')\n    and calls https://app.atera.com/api/v3/agents/machine/$ENV:COMPUTERNAME.\ntoken_model:\n  multiple_tokens: true\n  named: true\n  expiration: required\n  max_lifetime: 1 year from creation\n  ip_restriction:\n    supported: true\n    modes: [allow-all, specific-ips]\n  permissions:\n    modes: [full-access, custom-access]\n    granularity: per data domain\n    actions: [Read, Write, Delete]\n    note: >-\n      Custom access sets Read/Write/Delete independently for each of the twelve data\n      domains. This is a token permission model, not OAuth scopes — there is no\n      authorization server, no\
  \ consent screen and no scope string, so no scopes/\n      artifact is emitted.\n  rotation: >-\n    Tokens carry an operator-chosen expiration date (maximum one year), so rotation is\n    enforced by expiry rather than by a documented rotation procedure.\n  announced: >-\n    Multiple tokens with expiration dates, IP restrictions and permission scopes shipped\n    in 2026 (Release Notes: 2026), initially to new accounts only.\ndomains:\n- Agents\n- Alerts\n- Billing\n- Contacts\n- Contracts\n- Customers\n- CustomValues\n- Departments\n- Devices\n- KnowledgeBase\n- Rates\n- Tickets\naccess:\n  included_in_subscription: true\n  available_during_trial: false\n  note: >-\n    \"The API module in Atera is included as part of your subscription at no additional\n    cost. However, it's important to note that during the trial period, API access is\n    not available.\" — Atera API FAQ.\ngaps:\n- No OAuth 2.0 or OpenID Connect authorization server is published.\n- No /.well-known/openid-configuration\
  \ or /.well-known/oauth-authorization-server on\n  app.atera.com (probed 2026-08-06 — see well-known/atera-well-known.yml).\n- The interactive API reference cannot be read without an authenticated tenant token,\n  so the exact per-operation security requirements are not publicly verifiable.\nx-evidence:\n- {url: 'https://support.atera.com/hc/en-us/articles/219083397-Using-the-Atera-API', http_status: 200, fetched: '2026-08-06'}\n- {url: 'https://support.atera.com/hc/en-us/articles/11071761826844-API-FAQ', http_status: 200, fetched: '2026-08-06'}\n- {url: 'https://app.atera.com/api/v3/agents', http_status: 401, fetched: '2026-08-06', note: unauthenticated call returns 401 with empty body}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atera/refs/heads/main/authentication/atera-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- IT Management
- RMM
- PSA
- Help Desk
- Ticketing
- Patch Management
- Remote Monitoring
- Endpoint Management
- MSP
- Network Discovery
- Alerts
- Devices
- Billing
- Webhook
- Artificial Intelligence
---
