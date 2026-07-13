---
api_key_in: []
api_specs:
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Captures API
  slug: estuary-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Materializations API
  slug: estuary-materializations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Collections API
  slug: estuary-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Catalog Drafts API
  slug: estuary-catalog-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Publications API
  slug: estuary-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Connectors API
  slug: estuary-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Tenants & Billing API
  slug: estuary-tenants-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
- filename: estuary-openapi.yml
  format: yaml
  label: Estuary Auth & Tokens API
  slug: estuary-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/openapi/estuary-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Estuary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Estuary secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Estuary
provider_slug: estuary
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Access token obtained from /rpc/generate_access_token by exchanging a refresh token. Sent as Authorization: Bearer <access_token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/estuary-openapi.yml
  type: http
slug: estuary-authentication
source_filename: estuary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/estuary-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Access token obtained from /rpc/generate_access_token by exchanging a refresh\n    token. Sent as Authorization: Bearer <access_token>.'\n  sources:\n  - openapi/estuary-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estuary/refs/heads/main/authentication/estuary-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Integration
- Streaming ETL
- Change Data Capture
- CDC
- Real-Time Data
- Data Pipelines
---
