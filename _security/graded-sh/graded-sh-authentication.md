---
anonymous_access: false
api_key_in: []
api_specs:
- filename: graded-sh-services-api-openapi.yml
  format: yaml
  label: Graded Services API
  slug: graded-sh-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/graded-sh/openapi/graded-sh-services-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Graded Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graded secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Graded
provider_slug: graded-sh
scheme_count: 1
schemes:
- description: gwk_ agent key from POST /v1/accounts (or gwo_ owner key where noted). See /auth.md.
  name: bearer
  scheme: bearer
  sources:
  - openapi/graded-sh-openapi.yml
  type: http
slug: graded-sh-authentication
source_filename: graded-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/graded-sh-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: gwk_ agent key from POST /v1/accounts (or gwo_ owner key where noted). See /auth.md.\n  sources:\n  - openapi/graded-sh-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/graded-sh/authentication/graded-sh-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Payments
- Gateways
- API-Index
- AgentEconomy
---
