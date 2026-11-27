---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: CoreLoop Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoreLoop declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CoreLoop
provider_slug: coreloop-so
scheme_count: 1
schemes:
- applies_to:
  - https://coreloop.so/api/mcp/{slug}
  - https://coreloop.so/api/mcp/coreloop-directory
  - https://coreloop.so/api/a2a/{slug}
  - https://coreloop.so/api/a2a/coreloop-directory
  name: none (public agent endpoints)
  notes: Calls are rate limited per business slug and logged with a hashed agent identifier; unpublished profiles return an error before rate limiting.
  text: No authentication is required; the endpoint is public and secured by the gate chain described in the overview.
  type: none
slug: coreloop-so-authentication
source_filename: coreloop-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CoreLoop authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://coreloop.so/docs/mcp\ndocs: https://coreloop.so/docs/mcp\nrelated_docs:\n- https://coreloop.so/docs/protocols-overview\n- https://coreloop.so/docs/signing-in\nschemes:\n- name: none (public agent endpoints)\n  type: none\n  applies_to:\n  - https://coreloop.so/api/mcp/{slug}\n  - https://coreloop.so/api/mcp/coreloop-directory\n  - https://coreloop.so/api/a2a/{slug}\n  - https://coreloop.so/api/a2a/coreloop-directory\n  text: No authentication is required; the endpoint is public and secured by the gate chain described in the overview.\n  notes: Calls are rate limited per business slug and logged with a hashed agent identifier; unpublished profiles return an error before rate limiting.\ndashboard_sign_in:\n  docs: https://coreloop.so/docs/signing-in\n  methods:\n  - Email one-time 6-digit code\n  - Google, Microsoft, Facebook or Apple sign-in\n  - Passkey\n  - Optional two-factor authentication\
  \ (authenticator app)\n  text: There are no passwords on CoreLoop.\napi_access: Enterprise plans include \"API access\", arranged directly; no public documentation of the API's authentication was found (https://coreloop.so/docs/plans-and-billing).\n"
source_yaml_url: https://artifacts.apis.io/coreloop-so/authentication/coreloop-so-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Agents
- MCP
- A2A
- Llms.txt
- Business Directory
- Agent Discoverability
---
