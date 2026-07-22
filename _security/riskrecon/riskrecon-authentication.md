---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Riskrecon Authentication
name_suffix: Authentication
oauth_flows: []
overview: RiskRecon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RiskRecon
provider_slug: riskrecon
scheme_count: 1
schemes:
- bearer_format: JWT
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - live-probe:https://api.riskrecon.com/v1
  type: http
slug: riskrecon-authentication
source_filename: riskrecon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  Live probe of https://api.riskrecon.com/v1 (2026-07-21). Unauthenticated request to\n  /v1/toe/{toe} returned HTTP 401 with ReasonCode UNAUTHORIZED and Details \"Invalid JWT\",\n  confirming JWT bearer authentication.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  RiskRecon authenticates API calls with a JWT bearer token issued to the customer account.\n  The token is passed in the standard HTTP Authorization header as \"Authorization: Bearer <JWT>\".\n  Tokens are provisioned from the RiskRecon portal (portal.riskrecon.com). No OAuth 2.0 flow\n  or OpenID Connect discovery surface was found; there is no oauth2 authorization/token\n  endpoint published. Missing or invalid tokens return HTTP 401 with the RiskRecon error\n  envelope (ReasonCode UNAUTHORIZED, Details \"Invalid JWT\").\nschemes:\n- name: bearerAuth\n  type: http\n  scheme:\
  \ bearer\n  bearer_format: JWT\n  in: header\n  header: Authorization\n  sources:\n  - live-probe:https://api.riskrecon.com/v1\ndocs: https://api.riskrecon.com/v1/swagger/index.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riskrecon/refs/heads/main/authentication/riskrecon-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cybersecurity
- Security Ratings
- Third Party Risk
- Supply Chain Risk
- Risk Management
- GRC
- Vendor Monitoring
- Attack Surface
---
