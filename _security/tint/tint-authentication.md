---
api_key_in: []
api_specs:
- filename: tint-openapi.yml
  format: yaml
  label: Tint Programs API
  slug: tint-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Quotes API
  slug: tint-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Policies API
  slug: tint-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Claims API
  slug: tint-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Decisions API
  slug: tint-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Questionnaires API
  slug: tint-questionnaires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Webhooks API
  slug: tint-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tint secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tint
provider_slug: tint
scheme_count: 1
schemes:
- description: 'API token passed as "Authorization: Bearer ${API_TOKEN}". The token determines whether the request is routed to the sandbox or production environment.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tint-openapi.yml
  type: http
slug: tint-authentication
source_filename: tint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tint-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token passed as \"Authorization: Bearer ${API_TOKEN}\". The token determines\n    whether the request is routed to the sandbox or production environment.'\n  sources:\n  - openapi/tint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/authentication/tint-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Embedded Insurance
- InsurTech
- Insurance as a Service
- Protection
---
