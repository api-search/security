---
api_key_in: []
api_specs:
- filename: develop-health-openapi.yml
  format: yaml
  label: Develop Health Public API
  slug: develop-health-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/develop-health/refs/heads/main/openapi/develop-health-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Develop Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Develop Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Develop Health
provider_slug: develop-health
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is your auth token.
  name: FronteggJWTAuthentication
  scheme: bearer
  sources:
  - openapi/develop-health-openapi.yml
  type: http
slug: develop-health-authentication
source_filename: develop-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/develop-health-openapi.yml\ndocs: https://docs.develophealth.ai/api-reference/authentication\nnotes: >-\n  Identity is managed by Frontegg (login, sessions, MFA, SSO via the Develop\n  Health platform). API callers obtain a Frontegg-issued JWT from the platform\n  dashboard and present it as an HTTP bearer token (Authorization: Bearer <JWT>).\n  Suitable for server-to-server and third-party integrations. No OAuth2\n  scope/permission surface is documented.\nsummary:\n  types:\n  - http\n  provider: Frontegg\nschemes:\n- name: FronteggJWTAuthentication\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is\n    your auth token.\n  sources:\n  - openapi/develop-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/develop-health/refs/heads/main/authentication/develop-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Prior Authorization
- Benefit Verification
- Medication Access
- Insurance
- Health Tech
- Artificial Intelligence
---
