---
api_key_in: []
api_specs:
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel Metrics Queries API
  slug: propel-data-metrics-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel Data Pools API
  slug: propel-data-data-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel Data Sources API
  slug: propel-data-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel Applications and Policies API
  slug: propel-data-applications-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel OAuth2 Token API
  slug: propel-data-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Propel Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Propel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Propel
provider_slug: propel-data
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 client-credentials access token obtained from POST https://auth.us-east-2.propeldata.com/oauth2/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/propel-data-openapi.yml
  type: http
slug: propel-data-authentication
source_filename: propel-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/propel-data-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 client-credentials access token obtained from POST https://auth.us-east-2.propeldata.com/oauth2/token.\n  sources:\n  - openapi/propel-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/authentication/propel-data-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- GraphQL
- Data Warehouse
- Metrics
- Customer Facing Analytics
---
