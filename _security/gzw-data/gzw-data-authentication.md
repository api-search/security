---
api_key_in: []
api_specs:
- filename: spec
  format: yaml
  label: GZW Data API
  slug: gzw-data-api
  spec_type: OpenAPI
  url: https://gzw-data.dev/api/v1/spec
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Gzw Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: GZW Data API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: GZW Data API
provider_slug: gzw-data
scheme_count: 0
schemes: []
slug: gzw-data-authentication
source_filename: gzw-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://gzw-data.dev/docs/ (section \"Authentication — None, Public access, no API key\") + https://gzw-data.dev/llms.txt\ndocs: https://gzw-data.dev/docs/\nnote: >-\n  GZW Data is an unauthenticated public read-only API. The OpenAPI document declares NO\n  components.securitySchemes and no top-level security block, and the docs and llms.txt both\n  state plainly that authentication is none and no API key is required. This artifact records\n  a documented ABSENCE of authentication, not a gap in our research. Verified by anonymous\n  probe: GET https://gzw-data.dev/api/v1/weapons returned 200 with no credential supplied.\nmodel: none\napi_key_required: false\naccount_required: false\noauth2: false\nschemes: []\nevidence:\n- url: https://gzw-data.dev/api/v1/spec\n  status: 200\n  finding: no components.securitySchemes, no security block, 352 operations\n- url: https://gzw-data.dev/api/v1/weapons\n  status: 200\n  finding: 200\
  \ OK anonymously, no credential supplied\n- url: https://gzw-data.dev/docs/\n  status: 200\n  finding: 'docs state \"Authentication: None — Public access, no API key\"'\naccess_control:\n  mechanism: best-effort per-IP rate limiting\n  detail: See rate-limits/gzw-data-rate-limits.yml — 100 requests/minute/IP is the only access control.\ncors:\n  access_control_allow_origin: '*'\n  observed: 2026-08-26\n  note: Browser clients can call the API directly from any origin.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gzw-data/refs/heads/main/authentication/gzw-data-authentication.yml
summary_line: 0 schemes
tags:
- gaming
- video-games
- gray-zone-warfare
- game-data
- developer-tools
- open-data
- openapi
- weapons
- missions
- loot
- rest-api
- public-api
- no-auth
- read-only
- free-api
- community
---
