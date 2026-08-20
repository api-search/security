---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Osly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Osly secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Osly
provider_slug: osly
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeader
  note: 'The SDK throws AuthenticationError("Authentication required: Please provide an API key") before any request when no key is set — the REST surface has no anonymous mode.'
  parameter_name: X-API-Key
  required: true
  source: src/http/client.ts buildAuthHeaders()
  type: apiKey
- in: body
  name: SocketToken
  note: The Socket.IO surface carries the same key as a `token` field, both in the connection options and again inside the run_workflow payload.
  parameter_name: token
  required: true
  source: src/socket/connect.ts, src/socket/workflow.ts
  type: apiKey
slug: osly-authentication
source_filename: osly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: https://github.com/Osly-AI/Pocketflow-SDK/blob/main/src/http/client.ts\nderived_from: first-party SDK source published by Osly (github.com/Osly-AI); no OpenAPI or\n  developer documentation exists to derive from\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  oidc: false\n  mutual_tls: false\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  required: true\n  source: src/http/client.ts buildAuthHeaders()\n  note: >-\n    The SDK throws AuthenticationError(\"Authentication required: Please provide an API key\")\n    before any request when no key is set — the REST surface has no anonymous mode.\n- name: SocketToken\n  type: apiKey\n  in: body\n  parameter_name: token\n  required: true\n  source: src/socket/connect.ts, src/socket/workflow.ts\n  note: >-\n    The Socket.IO surface carries the same key as a `token` field, both in the connection\n    options and\
  \ again inside the run_workflow payload.\nkey_format:\n  prefix: pfl_\n  source: https://github.com/Osly-AI/Pocketflow-SDK#readme (\".env\" example shows\n    POCKETFLOW_API_KEY=pfl_your_api_key)\nkey_issuance:\n  console: https://platform.pocketflow.ai/settings/api\n  status: unreachable\n  note: >-\n    The README directs users to the PocketFlow dashboard settings page to mint a key.\n    platform.pocketflow.ai 301-redirects to app.osly.ai, which returns Cloudflare 522, so no\n    key can currently be issued.\nfailure_modes:\n- status: 401\n  meaning: authentication failed — key missing or invalid\n- status: 403\n  meaning: authentication failed — key rejected\ndocs: null\ndocs_note: >-\n  Osly publishes no authentication documentation page. This profile is derived entirely from\n  the company's own SDK source; nothing here was invented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osly/refs/heads/main/authentication/osly-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- Workflow-Automation
- No-Code
- Agents
- Lead Generation
- Productivity
- Integration
- Low-Code
---
