---
api_key_in:
- header
- body
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mosyle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mosyle secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mosyle
provider_slug: mosyle
scheme_count: 1
schemes:
- description: 'Per-account API access token (a JWT since 2024-02-08) generated in the Mosyle Business admin console. Required on every request. Observed live: a POST to https://businessapi.mosyle.com/v1/listdevices without it returns HTTP 401 {"error":"accessToken Required"}.'
  format: jwt
  in: header
  name: accessToken
  parameter_name: accessToken
  sources:
  - live-probe
  type: apiKey
slug: mosyle-authentication
source_filename: mosyle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://business.mosyle.com/ (feature listing \"Integrations with Google, Microsoft, Okta, AD & API\") + live probe of https://businessapi.mosyle.com/v1\ndocs: null\nsummary:\n  types: [apiKey]\n  api_key_in: [header, body]\n  oauth2_flows: []\n  notes: >-\n    The Mosyle Business API authenticates with an accessToken credential. Since\n    February 8, 2024 the accessToken is issued as a JSON Web Token (JWT) scoped\n    to a Mosyle Business account with permission to read/act on assets. The token\n    is supplied on each request; unauthenticated requests are rejected.\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter_name: accessToken\n  format: jwt\n  description: >-\n    Per-account API access token (a JWT since 2024-02-08) generated in the Mosyle\n    Business admin console. Required on every request. Observed live: a POST to\n    https://businessapi.mosyle.com/v1/listdevices without it returns HTTP\
  \ 401\n    {\"error\":\"accessToken Required\"}.\n  sources: [live-probe]\nevidence:\n- source: https://businessapi.mosyle.com/v1/listdevices\n  observed: 'HTTP 401 {\"error\":\"accessToken Required\"}'\n- source: web\n  observed: >-\n    Third-party integrations (Axonius, JupiterOne, Frontline, FMX) document\n    Mosyle Business API auth via an accessToken / JWT plus account credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosyle/refs/heads/main/authentication/mosyle-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Apple
- Device Management
- MDM
- Endpoint Security
- Identity
- SSO
- macOS
- iOS
- IT Operations
- Security
---
