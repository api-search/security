---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: opcreative-us-catalog-api-openapi.yml
  format: yaml
  label: opcreative-us Catalog API
  slug: opcreative-us-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opcreative-us/openapi/opcreative-us-catalog-api-openapi.yml
- filename: opcreative-us-me-api-openapi.yml
  format: yaml
  label: opcreative-us Me API
  slug: opcreative-us-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opcreative-us/openapi/opcreative-us-me-api-openapi.yml
- filename: opcreative-us-orders-api-openapi.yml
  format: yaml
  label: opcreative-us Orders API
  slug: opcreative-us-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opcreative-us/openapi/opcreative-us-orders-api-openapi.yml
- filename: opcreative-us-products-api-openapi.yml
  format: yaml
  label: opcreative-us Products API
  slug: opcreative-us-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opcreative-us/openapi/opcreative-us-products-api-openapi.yml
- filename: opcreative-us-stations-api-openapi.yml
  format: yaml
  label: opcreative-us Stations API
  slug: opcreative-us-stations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opcreative-us/openapi/opcreative-us-stations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: opcreative-us Authentication
name_suffix: Authentication
oauth_flows: []
overview: opcreative-us secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: opcreative-us
provider_slug: opcreative-us
scheme_count: 1
schemes:
- description: Create one in your dashboard under Profile → API.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/opcreative-us-openapi.json
  type: apiKey
slug: opcreative-us-authentication
source_filename: opcreative-us-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/opcreative-us-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Create one in your dashboard under Profile → API.\n  sources:\n  - openapi/opcreative-us-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/opcreative-us/authentication/opcreative-us-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
---
