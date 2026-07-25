---
api_key_in: []
api_specs:
- filename: tropic-contracts-api-openapi.yml
  format: yaml
  label: Tropic Contracts API
  slug: tropic-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/openapi/tropic-contracts-api-openapi.yml
- filename: tropic-requests-api-openapi.yml
  format: yaml
  label: Tropic Requests API
  slug: tropic-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/openapi/tropic-requests-api-openapi.yml
- filename: tropic-suppliers-api-openapi.yml
  format: yaml
  label: Tropic Suppliers API
  slug: tropic-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/openapi/tropic-suppliers-api-openapi.yml
- filename: tropic-users-api-openapi.yml
  format: yaml
  label: Tropic Users API
  slug: tropic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/openapi/tropic-users-api-openapi.yml
- filename: tropic-webhooks-api-openapi.yml
  format: yaml
  label: Tropic Webhooks API
  slug: tropic-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/openapi/tropic-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tropic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tropic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tropic
provider_slug: tropic
scheme_count: 1
schemes:
- description: API key issued from the Tropic settings panel
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tropic-openapi.yml
  type: http
slug: tropic-authentication
source_filename: tropic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tropic-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key issued from the Tropic settings panel\n  sources:\n  - openapi/tropic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/authentication/tropic-authentication.yml
summary_line: http · 1 scheme
tags:
- Benchmarking
- Contract Management
- Cost Optimization
- Procurement
- Renewals
- SaaS Management
- SaaS Procurement
- Spend Management
- Supplier Management
---
