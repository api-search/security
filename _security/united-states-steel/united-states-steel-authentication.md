---
api_key_in: []
api_specs:
- filename: united-states-steel-inventory-api-openapi.yml
  format: yaml
  label: United States Steel Inventory API
  slug: united-states-steel-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-steel/refs/heads/main/openapi/united-states-steel-inventory-api-openapi.yml
- filename: united-states-steel-orders-api-openapi.yml
  format: yaml
  label: United States Steel Orders API
  slug: united-states-steel-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-steel/refs/heads/main/openapi/united-states-steel-orders-api-openapi.yml
- filename: united-states-steel-shipments-api-openapi.yml
  format: yaml
  label: United States Steel Shipments API
  slug: united-states-steel-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-steel/refs/heads/main/openapi/united-states-steel-shipments-api-openapi.yml
- filename: united-states-steel-test-reports-api-openapi.yml
  format: yaml
  label: United States Steel Test Reports API
  slug: united-states-steel-test-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-steel/refs/heads/main/openapi/united-states-steel-test-reports-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: United States Steel Authentication
name_suffix: Authentication
oauth_flows: []
overview: United States Steel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: United States Steel
provider_slug: united-states-steel
scheme_count: 1
schemes:
- description: Bearer token authentication for SteelTrack API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/united-states-steel-steeltrack-openapi.yml
  type: http
slug: united-states-steel-authentication
source_filename: united-states-steel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/united-states-steel-steeltrack-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication for SteelTrack API.\n  sources:\n  - openapi/united-states-steel-steeltrack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-steel/refs/heads/main/authentication/united-states-steel-authentication.yml
summary_line: http · 1 scheme
tags:
- Steel
- Manufacturing
- Automotive
- Construction
- Energy
- Supply Chain
- Fortune 500
---
