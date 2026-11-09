---
anonymous_access: false
api_key_in:
- cookie
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Aeroz Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aeroz secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aeroz
provider_slug: aeroz-io
scheme_count: 2
schemes:
- description: Your Aeroz API key (ak_sbx_… or ak_live_…). Each operation names the one scope a key needs in its security requirement and in x-required-scope; a key without it gets 403 insufficient_scope with scope_needed. GET /v1/keys lists every scope.
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/aeroz-io-openapi.json
  type: http
- description: A signed-in person in the dashboard, with the company named in the X-Aeroz-Workspace header. Single sign-on and SCIM settings accept only this, from an owner or admin — never an API key.
  in: cookie
  name: SessionAuth
  parameter: __Host-aeroz_session
  sources:
  - openapi/aeroz-io-openapi.json
  type: apiKey
slug: aeroz-io-authentication
source_filename: aeroz-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/aeroz-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: Your Aeroz API key (ak_sbx_… or ak_live_…). Each operation names the one scope\n    a key needs in its security requirement and in x-required-scope; a key without it gets 403\n    insufficient_scope with scope_needed. GET /v1/keys lists every scope.\n  sources:\n  - openapi/aeroz-io-openapi.json\n- name: SessionAuth\n  type: apiKey\n  in: cookie\n  parameter: __Host-aeroz_session\n  description: A signed-in person in the dashboard, with the company named in the X-Aeroz-Workspace\n    header. Single sign-on and SCIM settings accept only this, from an owner or admin — never\n    an API key.\n  sources:\n  - openapi/aeroz-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aeroz-io/authentication/aeroz-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Supply Chain
- Traceability
- Authentication
- Compliance
- NFC
---
