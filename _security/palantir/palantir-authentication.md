---
api_key_in: []
api_specs:
- filename: palantir-openapi.yml
  format: yaml
  label: Palantir Foundry API
  slug: palantir-foundry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palantir/refs/heads/main/openapi/palantir-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Palantir Authentication
name_suffix: Authentication
oauth_flows: []
overview: Palantir secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Palantir
provider_slug: palantir
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token. The token must be passed as an `Authorization` header using the `Bearer` authentication scheme. Foundry supports user-generated API tokens (for development), Authorization Code grant, and Client Credentials grant.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/palantir-openapi.yml
  type: http
slug: palantir-authentication
source_filename: palantir-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/palantir-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token. The token must be passed as an `Authorization` header\n    using the `Bearer` authentication scheme. Foundry supports user-generated API tokens (for\n    development), Authorization Code grant, and Client Credentials grant.\n  sources:\n  - openapi/palantir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palantir/refs/heads/main/authentication/palantir-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Platform
- Data Analytics
- Enterprise
- Government
---
