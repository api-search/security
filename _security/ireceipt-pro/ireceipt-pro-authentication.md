---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ireceipt-pro-jpg-api-openapi.yml
  format: yaml
  label: ireceipt-pro /jpg API
  slug: ireceipt-pro-jpg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-jpg-api-openapi.yml
- filename: ireceipt-pro-pdf-api-openapi.yml
  format: yaml
  label: ireceipt-pro /pdf API
  slug: ireceipt-pro-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-pdf-api-openapi.yml
- filename: ireceipt-pro-ping-api-openapi.yml
  format: yaml
  label: ireceipt-pro /ping API
  slug: ireceipt-pro-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-ping-api-openapi.yml
- filename: ireceipt-pro-png-api-openapi.yml
  format: yaml
  label: ireceipt-pro /png API
  slug: ireceipt-pro-png-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-png-api-openapi.yml
- filename: ireceipt-pro-webp-api-openapi.yml
  format: yaml
  label: ireceipt-pro /webp API
  slug: ireceipt-pro-webp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-webp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ireceipt Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: ireceipt-pro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ireceipt-pro
provider_slug: ireceipt-pro
scheme_count: 1
schemes:
- name: accessBearerAuth
  scheme: bearer
  sources:
  - openapi/ireceipt-pro-openapi.yml
  type: http
slug: ireceipt-pro-authentication
source_filename: ireceipt-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/ireceipt-pro-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessBearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ireceipt-pro-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/ireceipt-pro/authentication/ireceipt-pro-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- API
- PDF
- ImageGeneration
- Templates
---
