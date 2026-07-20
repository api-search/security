---
api_key_in:
- header
api_specs:
- filename: cycognito-v1-openapi-original.json
  format: json
  label: CyCognito API V1
  slug: cycognito-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-v1-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cycognito Authentication
name_suffix: Authentication
oauth_flows: []
overview: CyCognito secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CyCognito
provider_slug: cycognito
scheme_count: 1
schemes:
- in: header
  name: apiAuth
  parameter: Authorization
  sources:
  - openapi/cycognito-v1-openapi-original.json
  type: apiKey
slug: cycognito-authentication
source_filename: cycognito-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cycognito-v1-openapi-original.json\ndocs: https://api.platform.cycognito.com/v1/docs/index.html\nnotes: API V1 authenticates with a user-generated API key in the Authorization header. Platform SSO is separately handled by an Auth0 tenant (auth.cycognito.com, OpenID Connect) and is not the API-key surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/cycognito-v1-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/authentication/cycognito-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Attack Surface Management
- Exposure Management
- Security
- Vulnerability Management
- Cloud Security
- API Security
---
