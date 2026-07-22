---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Zenput Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenput secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zenput
provider_slug: zenput
scheme_count: 1
schemes:
- description: Per-user API token passed in the X-API-TOKEN request header on every call. A user generates the token from their account settings at https://www.zenput.com/settings. There is no OAuth flow documented; the token is a static per-user secret scoped to that user's company access.
  in: header
  name: apiToken
  parameter_name: X-API-TOKEN
  sources:
  - https://developer.zenput.com/docs/introduction
  type: apiKey
slug: zenput-authentication
source_filename: zenput-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.zenput.com/docs/introduction\ndocs: https://developer.zenput.com/docs/introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter_name: X-API-TOKEN\n  description: >-\n    Per-user API token passed in the X-API-TOKEN request header on every call.\n    A user generates the token from their account settings at\n    https://www.zenput.com/settings. There is no OAuth flow documented; the\n    token is a static per-user secret scoped to that user's company access.\n  sources:\n  - https://developer.zenput.com/docs/introduction\nnotes: >-\n  Token-based header authentication only. No documented OAuth2, OpenID Connect,\n  HTTP Basic/Bearer, or mutualTLS scheme, so no scopes/ artifact is emitted\n  (key-auth providers have no OAuth scope surface).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenput/refs/heads/main/authentication/zenput-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Restaurant Operations
- Operations Execution
- Food Safety
- Compliance
- Task Management
- Convenience Stores
- Field Operations
- Restaurant Technology
---
