---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shiprust-account-api-openapi.yml
  format: yaml
  label: ShipRust Account API
  slug: shiprust-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shiprust/openapi/shiprust-account-api-openapi.yml
- filename: shiprust-projects-api-openapi.yml
  format: yaml
  label: ShipRust Projects API
  slug: shiprust-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shiprust/openapi/shiprust-projects-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Shiprust Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShipRust secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ShipRust
provider_slug: shiprust
scheme_count: 1
schemes:
- bearerFormat: sr_<64 hex characters>
  description: A personal API key from Settings, or an OAuth 2.1 access token obtained through the authorization server described at /.well-known/oauth-authorization-server. Cookies are never accepted.
  name: api_key
  scheme: bearer
  sources:
  - openapi/shiprust-openapi.json
  type: http
slug: shiprust-authentication
source_filename: shiprust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/shiprust-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  bearerFormat: sr_<64 hex characters>\n  description: A personal API key from Settings, or an OAuth 2.1 access token obtained through\n    the authorization server described at /.well-known/oauth-authorization-server. Cookies are\n    never accepted.\n  sources:\n  - openapi/shiprust-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/shiprust/authentication/shiprust-authentication.yml
summary_line: http · 1 scheme
tags:
- Rust
- SaaS
- Starter
- Axum
- PostgreSQL
---
