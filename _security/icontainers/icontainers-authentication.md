---
api_key_in: []
api_specs:
- filename: icontainers-bookings-api-openapi.yml
  format: yaml
  label: iContainers Bookings API
  slug: icontainers-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icontainers/refs/heads/main/openapi/icontainers-bookings-api-openapi.yml
- filename: icontainers-documents-api-openapi.yml
  format: yaml
  label: iContainers Documents API
  slug: icontainers-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icontainers/refs/heads/main/openapi/icontainers-documents-api-openapi.yml
- filename: icontainers-places-api-openapi.yml
  format: yaml
  label: iContainers Places API
  slug: icontainers-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icontainers/refs/heads/main/openapi/icontainers-places-api-openapi.yml
- filename: icontainers-quotes-api-openapi.yml
  format: yaml
  label: iContainers Quotes API
  slug: icontainers-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icontainers/refs/heads/main/openapi/icontainers-quotes-api-openapi.yml
- filename: icontainers-rates-api-openapi.yml
  format: yaml
  label: iContainers Rates API
  slug: icontainers-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icontainers/refs/heads/main/openapi/icontainers-rates-api-openapi.yml
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
- Track And Trace
---
