---
api_key_in: []
api_specs:
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Catalog API
  slug: up42-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Tasking API
  slug: up42-tasking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Orders API
  slug: up42-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Storage Assets API
  slug: up42-storage-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 STAC Data Management API
  slug: up42-stac-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Processing API
  slug: up42-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Webhooks API
  slug: up42-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
- filename: up42-openapi.yml
  format: yaml
  label: UP42 Workspaces and Account API
  slug: up42-workspaces-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/openapi/up42-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Up42 Authentication
name_suffix: Authentication
oauth_flows: []
overview: UP42 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UP42
provider_slug: up42
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth2 Bearer access token. Obtain a token from a UP42 API key or account credentials via https://auth.up42.com/realms/public/protocol/openid-connect/token (client_id up42-api). Access tokens are short-lived (about 5 minutes); refresh as needed. Pass as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/up42-openapi.yml
  type: http
slug: up42-authentication
source_filename: up42-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/up42-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 Bearer access token. Obtain a token from a UP42 API key or account credentials\n    via https://auth.up42.com/realms/public/protocol/openid-connect/token (client_id up42-api).\n    Access tokens are short-lived (about 5 minutes); refresh as needed. Pass as `Authorization:\n    Bearer [example key]`.'\n  sources:\n  - openapi/up42-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/authentication/up42-authentication.yml
summary_line: http · 1 scheme
tags:
- Geospatial
- Earth Observation
- Satellite Imagery
- Remote Sensing
- STAC
- Tasking
- Catalog
- Airbus
---
