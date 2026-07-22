---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Vev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vev secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vev
provider_slug: vev
scheme_count: 1
schemes:
- description: API key created in the Vev Design Editor under user profile, scoped to the relevant permissions. The key is valid forever until revoked. Sent as the x-vev-key header on every request to https://api.vev.design.
  in: header
  introspection_endpoint: https://api.vev.design/api-key/introspection
  name: vevApiKey
  parameter_name: x-vev-key
  scopes_note: API keys are created "with the relevant scope"; a documented scope reference was not found.
  sources:
  - https://developer.vev.design/api/auth
  type: apiKey
slug: vev-authentication
source_filename: vev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.vev.design/api/auth\ndocs: https://developer.vev.design/api/auth\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: vevApiKey\n  type: apiKey\n  in: header\n  parameter_name: x-vev-key\n  description: >-\n    API key created in the Vev Design Editor under user profile, scoped to the\n    relevant permissions. The key is valid forever until revoked. Sent as the\n    x-vev-key header on every request to https://api.vev.design.\n  scopes_note: API keys are created \"with the relevant scope\"; a documented scope reference was not found.\n  introspection_endpoint: https://api.vev.design/api-key/introspection\n  sources: [https://developer.vev.design/api/auth]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vev/refs/heads/main/authentication/vev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Design Tech
- No-Code
- Web Design
- CMS
- Website Builder
- Webhooks
- React Components
- Developer Tools
---
