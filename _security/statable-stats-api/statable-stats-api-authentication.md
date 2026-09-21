---
anonymous_access: false
api_key_in: []
api_specs:
- filename: statable-stats-api-openapi.yml
  format: yaml
  label: Statable Stats API
  slug: statable-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statable-stats-api/refs/heads/main/openapi/statable-stats-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Statable Stats Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Statable Stats API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Statable Stats API
provider_slug: statable-stats-api
scheme_count: 1
schemes:
- bearerFormat: stbl_<secret>
  description: A key minted in Settings → API. All tokens start with `stbl_`. Missing, malformed, invalid, expired, or revoked → 401. Every operation in this spec requires the key's `read` scope; without it → 403 `insufficient_scope`.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/statable-stats-api-openapi.yml
  type: http
slug: statable-stats-api-authentication
source_filename: statable-stats-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: derived\nsource: openapi/statable-stats-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: stbl_<secret>\n  description: A key minted in Settings → API. All tokens start with `stbl_`. Missing, malformed,\n    invalid, expired, or revoked → 401. Every operation in this spec requires the key's `read`\n    scope; without it → 403 `insufficient_scope`.\n  sources:\n  - openapi/statable-stats-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statable-stats-api/refs/heads/main/authentication/statable-stats-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Web Analytics
- Cookieless
- Privacy
- GDPR
- OpenAPI
- MCP
- llms-txt
- EU-hosted
---
