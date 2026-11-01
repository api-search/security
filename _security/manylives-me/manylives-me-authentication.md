---
anonymous_access: false
api_key_in: []
api_specs:
- filename: manylives-me-buyers-api-openapi.yml
  format: yaml
  label: manylives-me Buyers API
  slug: manylives-me-buyers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/manylives-me/openapi/manylives-me-buyers-api-openapi.yml
- filename: manylives-me-discovery-api-openapi.yml
  format: yaml
  label: manylives-me Discovery API
  slug: manylives-me-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/manylives-me/openapi/manylives-me-discovery-api-openapi.yml
- filename: manylives-me-members-api-openapi.yml
  format: yaml
  label: manylives-me Members API
  slug: manylives-me-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/manylives-me/openapi/manylives-me-members-api-openapi.yml
- filename: manylives-me-paid-api-openapi.yml
  format: yaml
  label: manylives-me Paid API
  slug: manylives-me-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/manylives-me/openapi/manylives-me-paid-api-openapi.yml
- filename: manylives-me-sellers-api-openapi.yml
  format: yaml
  label: manylives-me Sellers API
  slug: manylives-me-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/manylives-me/openapi/manylives-me-sellers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Manylives Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: manylives-me secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: manylives-me
provider_slug: manylives-me
scheme_count: 1
schemes:
- description: member_secret from registration (ss_<member_id>_<64 hex>).
  name: member
  scheme: bearer
  sources:
  - openapi/manylives-me-openapi.json
  type: http
slug: manylives-me-authentication
source_filename: manylives-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/manylives-me-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: member\n  type: http\n  scheme: bearer\n  description: member_secret from registration (ss_<member_id>_<64 hex>).\n  sources:\n  - openapi/manylives-me-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/manylives-me/authentication/manylives-me-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Payments
- Crypto
- Tools
---
