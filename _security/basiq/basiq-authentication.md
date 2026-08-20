---
api_key_in: []
api_specs:
- filename: basiq-accounts-api-openapi.yml
  format: yaml
  label: Basiq Accounts API
  slug: basiq-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-accounts-api-openapi.yml
- filename: basiq-affordability-api-openapi.yml
  format: yaml
  label: Basiq Affordability API
  slug: basiq-affordability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-affordability-api-openapi.yml
- filename: basiq-authentication-api-openapi.yml
  format: yaml
  label: Basiq Authentication API
  slug: basiq-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-authentication-api-openapi.yml
- filename: basiq-connections-api-openapi.yml
  format: yaml
  label: Basiq Connections API
  slug: basiq-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-connections-api-openapi.yml
- filename: basiq-transactions-api-openapi.yml
  format: yaml
  label: Basiq Transactions API
  slug: basiq-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-transactions-api-openapi.yml
- filename: basiq-users-api-openapi.yml
  format: yaml
  label: Basiq Users API
  slug: basiq-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/openapi/basiq-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Basiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basiq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Basiq
provider_slug: basiq
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/basiq-api-openapi.yml
  type: http
slug: basiq-authentication
source_filename: basiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/basiq-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/basiq-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/authentication/basiq-authentication.yml
summary_line: http · 1 scheme
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transaction
---
