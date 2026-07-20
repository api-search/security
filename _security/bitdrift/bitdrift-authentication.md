---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bitdrift Authentication
name_suffix: Authentication
oauth_flows: []
overview: bitdrift secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: bitdrift
provider_slug: bitdrift
scheme_count: 1
schemes:
- description: API key minted via `bd key create api` or the AdminService CreateKey method. Sent on every request in the x-bitdrift-api-key header. Keys carry explicit permissions for public-API access.
  in: header
  name: ApiKeyAuth
  parameter_name: x-bitdrift-api-key
  sources:
  - grpc/src/bitdrift/public/unary/admin/v1/keys.proto
  type: apiKey
slug: bitdrift-authentication
source_filename: bitdrift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.bitdrift.io/api-guide/calling-the-api.html\ndocs: https://docs.bitdrift.io/api-guide/calling-the-api.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The public API authenticates with an API key sent in the x-bitdrift-api-key header. JWT-\n    authenticated requests against the public API are not supported. The bd CLI additionally offers a\n    browser-based user login (bd auth) for interactive/user-authenticated access; that login flow is\n    a CLI capability, not a public-API auth mode.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-bitdrift-api-key\n  description: >-\n    API key minted via `bd key create api` or the AdminService CreateKey method. Sent on every\n    request in the x-bitdrift-api-key header. Keys carry explicit permissions for public-API access.\n  sources: [grpc/src/bitdrift/public/unary/admin/v1/keys.proto]\n\
  key_management:\n  create_cli: bd key create api\n  create_api: AdminService.CreateKey\n  list_api: AdminService.GetKeys\n  revoke_api: AdminService.RevokeKey\n  env_var: BD_API_KEY\ncli_user_login:\n  command: bd auth\n  mechanism: browser-based SaaS login (user-authenticated)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitdrift/refs/heads/main/authentication/bitdrift-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Developer Tools
- Observability
- Mobile
- Monitoring
- Logging
- Crash Reporting
- Session Replay
- SDK
- gRPC
- Telemetry
---
