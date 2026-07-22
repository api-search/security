---
api_key_in: []
api_specs:
- filename: vts-openapi.yml
  format: yaml
  label: VTS Lease API
  slug: vts-lease-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vts/refs/heads/main/openapi/vts-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Vts Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: VTS secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: VTS
provider_slug: vts
scheme_count: 2
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/vts-openapi.yml
  type: http
- description: OAuth 2.0 Authorization Code flow with PKCE (VTS Activate / OIDC).
  flows:
  - authorizationUrl: https://sandbox.vts.com/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://sandbox.vts.com/oauth/token
  name: oauth2
  sources:
  - openapi/vts-openapi.yml
  type: oauth2
slug: vts-authentication
source_filename: vts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vts-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/vts-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.vts.com/oauth/authorize\n    tokenUrl: https://sandbox.vts.com/oauth/token\n    scopes: 4\n  description: OAuth 2.0 Authorization Code flow with PKCE (VTS Activate / OIDC).\n  sources:\n  - openapi/vts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vts/refs/heads/main/authentication/vts-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Commercial Real Estate
- PropTech
- Real Estate
- Leasing
- Asset Management
- Property Management
- Tenant Experience
---
