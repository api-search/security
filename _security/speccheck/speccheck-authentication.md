---
api_key_in: []
api_specs:
- filename: speccheck-openapi.yml
  format: yaml
  label: SpecCheck API
  slug: speccheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speccheck/refs/heads/main/openapi/speccheck-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Speccheck Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpecCheck secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpecCheck
provider_slug: speccheck
scheme_count: 1
schemes:
- description: Bearer token obtained from POST /v1/oauth/token using client credentials. Tokens expire after 24 hours.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/speccheck-openapi.yml
  type: http
slug: speccheck-authentication
source_filename: speccheck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/speccheck-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from POST /v1/oauth/token using client credentials. Tokens\n    expire after 24 hours.\n  sources:\n  - openapi/speccheck-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speccheck/refs/heads/main/authentication/speccheck-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise Saas
- Optical
- Eyewear
- Eyecare
- Optical Labs
- Prescriptions
- Ordering
- Healthcare
---
