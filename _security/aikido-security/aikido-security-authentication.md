---
api_key_in: []
api_specs:
- filename: getopenapispec
  format: yaml
  label: Aikido Security REST API
  slug: aikido-rest-api
  spec_type: OpenAPI
  url: https://apidocs.aikido.dev/reference/getopenapispec
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aikido Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aikido Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aikido Security
provider_slug: aikido-security
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer access token obtained via POST https://app.aikido.dev/api/oauth/token

    with grant_type=client_credentials and Basic auth (client_id:client_secret).'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/aikido-security-openapi.yml
  type: http
slug: aikido-security-authentication
source_filename: aikido-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aikido-security-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Bearer access token obtained via POST https://app.aikido.dev/api/oauth/token\n    with grant_type=client_credentials and Basic auth (client_id:client_secret).\n  sources:\n  - openapi/aikido-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/authentication/aikido-security-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Pentesting
- API Security
- Application Security
- Cloud Security
- Compliance
- DAST
- Developer-First
- IaC Scanning
- SAST
- SCA
- Secret Detection
---
