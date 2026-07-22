---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Vertical Bar Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vertical Bar Inc. secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vertical Bar Inc.
provider_slug: vertical-bar-inc
scheme_count: 1
schemes:
- evidence: GET https://api.vertical.bar/ -> 401 {"message":"Invalid authorization header"}
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - live-probe
  type: http
slug: vertical-bar-inc-authentication
source_filename: vertical-bar-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: live probe of https://api.vertical.bar/ (unauthenticated 401 response)\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    No public OpenAPI or authentication documentation is published. The production\n    API host api.vertical.bar returns HTTP 401 with\n    {\"error\":{\"code\":401,\"message\":\"Invalid authorization header\"}} to\n    unauthenticated requests, indicating a bearer token supplied via the standard\n    Authorization request header (server: uvicorn / FastAPI-style). A gated\n    /.well-known/openid-configuration endpoint (307 to /login on the CrossCheck app\n    host, 401 on the API host) suggests an OIDC-based login for the app.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  evidence: 'GET https://api.vertical.bar/ -> 401 {\"message\":\"Invalid authorization header\"}'\n  sources: [live-probe]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertical-bar-inc/refs/heads/main/authentication/vertical-bar-inc-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- NetSuite
- DevOps
- ERP
- Change Management
- Process Mining
- Configuration Management
- Manufacturing
---
