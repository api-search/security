---
api_key_in: []
api_specs:
- filename: wove-authentication-api-openapi.yml
  format: yaml
  label: Wove Authentication API
  slug: wove-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-authentication-api-openapi.yml
- filename: wove-documents-api-openapi.yml
  format: yaml
  label: Wove Documents API
  slug: wove-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-documents-api-openapi.yml
- filename: wove-query-bank-api-openapi.yml
  format: yaml
  label: Wove Query Bank API
  slug: wove-query-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-query-bank-api-openapi.yml
- filename: wove-rates-api-openapi.yml
  format: yaml
  label: Wove Rates API
  slug: wove-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-rates-api-openapi.yml
- filename: wove-shipments-api-openapi.yml
  format: yaml
  label: Wove Shipments API
  slug: wove-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-shipments-api-openapi.yml
- filename: wove-sources-api-openapi.yml
  format: yaml
  label: Wove Sources API
  slug: wove-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-sources-api-openapi.yml
- filename: wove-tariffs-api-openapi.yml
  format: yaml
  label: Wove Tariffs API
  slug: wove-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-tariffs-api-openapi.yml
- filename: wove-testing-api-openapi.yml
  format: yaml
  label: Wove Testing API
  slug: wove-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-testing-api-openapi.yml
- filename: wove-tms-organizations-api-openapi.yml
  format: yaml
  label: Wove TMS Organizations API
  slug: wove-tms-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-tms-organizations-api-openapi.yml
- filename: wove-webhooks-api-openapi.yml
  format: yaml
  label: Wove Webhooks API
  slug: wove-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wove secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wove
provider_slug: wove
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token obtained from /auth/token endpoint
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wove-external-api-openapi-original.yml
  type: http
slug: wove-authentication
source_filename: wove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wove-external-api-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token obtained from /auth/token endpoint\n  sources:\n  - openapi/wove-external-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/authentication/wove-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
