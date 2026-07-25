---
api_key_in: []
api_specs:
- filename: octo-availability-api-openapi.yml
  format: yaml
  label: Open Connectivity for Tours, Activities, and Attractions Availability API
  slug: octo-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octo/refs/heads/main/openapi/octo-availability-api-openapi.yml
- filename: octo-bookings-api-openapi.yml
  format: yaml
  label: Open Connectivity for Tours, Activities, and Attractions Bookings API
  slug: octo-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octo/refs/heads/main/openapi/octo-bookings-api-openapi.yml
- filename: octo-products-api-openapi.yml
  format: yaml
  label: Open Connectivity for Tours, Activities, and Attractions Products API
  slug: octo-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octo/refs/heads/main/openapi/octo-products-api-openapi.yml
- filename: octo-supplier-api-openapi.yml
  format: yaml
  label: Open Connectivity for Tours, Activities, and Attractions Supplier API
  slug: octo-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octo/refs/heads/main/openapi/octo-supplier-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Octo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Connectivity for Tours, Activities, and Attractions secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open Connectivity for Tours, Activities, and Attractions
provider_slug: octo
scheme_count: 1
schemes:
- name: Auth
  scheme: bearer
  sources:
  - openapi/octo-openapi-original.yml
  type: http
slug: octo-authentication
source_filename: octo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/octo-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Auth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/octo-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octo/refs/heads/main/authentication/octo-authentication.yml
summary_line: http · 1 scheme
tags:
- Activities
- Attractions
- Open Standard
- Tours
- Travel
---
