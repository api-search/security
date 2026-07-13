---
api_key_in:
- cookie
api_specs:
- filename: mcafee-epo-openapi.yml
  format: yaml
  label: McAfee ePO API
  slug: mcafee-epo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/openapi/mcafee-epo-openapi.yml
- filename: mcafee-mvision-openapi.yml
  format: yaml
  label: McAfee MVISION API
  slug: mcafee-mvision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/openapi/mcafee-mvision-openapi.yml
- filename: mcafee-web-gateway-openapi.yml
  format: yaml
  label: McAfee Web Gateway API
  slug: mcafee-web-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/openapi/mcafee-web-gateway-openapi.yml
- filename: mcafee-esm-openapi.yml
  format: yaml
  label: McAfee ESM API
  slug: mcafee-esm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/openapi/mcafee-esm-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mcafee Authentication
name_suffix: Authentication
oauth_flows: []
overview: McAfee (Trellix) secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: McAfee (Trellix)
provider_slug: mcafee
scheme_count: 4
schemes:
- description: HTTP Basic authentication using ePO administrator credentials. Credentials are transmitted as a Base64-encoded username:password pair.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mcafee-epo-openapi.yml
  type: http
- description: Session token obtained from the login endpoint
  in: cookie
  name: sessionAuth
  parameter: JWTToken
  sources:
  - openapi/mcafee-esm-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 bearer token from client credentials grant
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mcafee-mvision-openapi.yml
  type: http
- description: Session cookie obtained from the login endpoint
  in: cookie
  name: cookieAuth
  parameter: JSESSIONID
  sources:
  - openapi/mcafee-web-gateway-openapi.yml
  type: apiKey
slug: mcafee-authentication
source_filename: mcafee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mcafee-epo-openapi.yml, openapi/mcafee-esm-openapi.yml, openapi/mcafee-mvision-openapi.yml,\n  openapi/mcafee-web-gateway-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using ePO administrator credentials. Credentials are\n    transmitted as a Base64-encoded username:password pair.\n  sources:\n  - openapi/mcafee-epo-openapi.yml\n- name: sessionAuth\n  type: apiKey\n  in: cookie\n  parameter: JWTToken\n  description: Session token obtained from the login endpoint\n  sources:\n  - openapi/mcafee-esm-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token from client credentials grant\n  sources:\n  - openapi/mcafee-mvision-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: JSESSIONID\n  description:\
  \ Session cookie obtained from the login endpoint\n  sources:\n  - openapi/mcafee-web-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/authentication/mcafee-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Antivirus
- Cybersecurity
- Endpoint Protection
- Security
- Threat Intelligence
---
