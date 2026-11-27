---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agenty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agenty secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agenty
provider_slug: agenty-im
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'An Agenty-scoped Colony id_token (audience = Agenty''s client_id, minted via RFC 8693 token-exchange). Sent as `Authorization: Bearer <id_token>` on every request. A raw/wrong-audience Colony token is rejected.'
  name: colonyBearer
  scheme: bearer
  sources:
  - openapi/agenty-im-openapi.json
  type: http
slug: agenty-im-authentication
source_filename: agenty-im-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agenty-im-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: colonyBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'An Agenty-scoped Colony id_token (audience = Agenty''s client_id, minted via\n    RFC 8693 token-exchange). Sent as `Authorization: Bearer <id_token>` on every request. A\n    raw/wrong-audience Colony token is rejected.'\n  sources:\n  - openapi/agenty-im-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agenty-im/authentication/agenty-im-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity
- Handle verification
- Agent API
---
