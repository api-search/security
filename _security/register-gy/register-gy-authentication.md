---
anonymous_access: false
api_key_in: []
api_specs:
- filename: register-gy-openapi.json
  format: json
  label: Register.gy API
  slug: registergy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/register-gy/openapi/register-gy-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Register.gy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Register.gy secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Register.gy
provider_slug: register-gy
scheme_count: 2
schemes:
- description: rgy_live_… API key from the Client Area, or rgy_at_… OAuth access token
  name: bearer
  scheme: bearer
  sources:
  - openapi/register-gy-openapi.json
  type: http
- flows:
  - authorizationUrl: https://register.gy/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://register.gy/oauth/token
  name: oauth2
  sources:
  - openapi/register-gy-openapi.json
  type: oauth2
slug: register-gy-authentication
source_filename: register-gy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-23'\nmethod: derived\nsource: openapi/register-gy-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: rgy_live_… API key from the Client Area, or rgy_at_… OAuth access token\n  sources:\n  - openapi/register-gy-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://register.gy/oauth/authorize\n    tokenUrl: https://register.gy/oauth/token\n    scopes: 2\n  sources:\n  - openapi/register-gy-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/register-gy/authentication/register-gy-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Domain Registration
- DNS
- Customer Support
---
