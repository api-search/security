---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Andpad Authentication
name_suffix: Authentication
oauth_flows: []
overview: ANDPAD declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ANDPAD
provider_slug: andpad
scheme_count: 1
schemes:
- detail: OAuth2 partner-app authorization brokered through the ANDPAD App Market; access tokens are presented as bearer credentials to api.andpad.jp/v1.
  endpoints_public: false
  name: andpad_app_market
  scopes_documented: false
  type: oauth2
slug: andpad-authentication
source_filename: andpad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.andpad.jp/\napi: ANDPAD API\nbase_url: https://api.andpad.jp/v1\nsummary: >-\n  ANDPAD exposes its REST API to partners through the ANDPAD App Market (アプリマーケット). Partner\n  applications are authorized via OAuth and call api.andpad.jp with a bearer access token. The\n  full OAuth authorization/token endpoints, client-registration flow, and scope catalog are\n  gated behind the developer/partner program and are not published on the public site, so they\n  are not enumerated here (no fabrication).\nschemes:\n  - type: oauth2\n    name: andpad_app_market\n    detail: >-\n      OAuth2 partner-app authorization brokered through the ANDPAD App Market; access tokens are\n      presented as bearer credentials to api.andpad.jp/v1.\n    scopes_documented: false\n    endpoints_public: false\nevidence:\n  - source: https://developer.andpad.jp/\n    kind: developer portal (ANDPAD API / App Market integration program)\n\
  \  - source: https://api.andpad.jp/v1/self\n    kind: protected resource returns 404/JSON to unauthenticated callers\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andpad/refs/heads/main/authentication/andpad-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Technology
- Construction
- Construction Management
- Construction DX
- SaaS
- Project Management
- Japan
- API
---
