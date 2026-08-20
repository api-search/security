---
api_key_in: []
api_specs:
- filename: icontainers-brutus-openapi.yml
  format: yaml
  label: iContainers Brutus API
  slug: icontainers-brutus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icontainers/refs/heads/main/openapi/icontainers-brutus-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Icontainers Authentication
name_suffix: Authentication
oauth_flows: []
overview: iContainers secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iContainers
provider_slug: icontainers
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/icontainers-brutus-openapi.yml
  type: http
slug: icontainers-authentication
source_filename: icontainers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: derived\nsource: openapi/icontainers-brutus-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/icontainers-brutus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icontainers/refs/heads/main/authentication/icontainers-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Marketplace
- Logistics
- Freight
- Shipping
- Ocean Freight
- Air Freight
- Supply Chain
- Customs
- Freight Quoting
- Container Shipping
- Track and Trace
---
