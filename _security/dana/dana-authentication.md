---
api_key_in:
- header
api_specs:
- filename: dana-availability-api-openapi.yml
  format: yaml
  label: Dana Availability API
  slug: dana-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-availability-api-openapi.yml
- filename: dana-orders-api-openapi.yml
  format: yaml
  label: Dana Orders API
  slug: dana-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-orders-api-openapi.yml
- filename: dana-parts-api-openapi.yml
  format: yaml
  label: Dana Parts API
  slug: dana-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-parts-api-openapi.yml
- filename: dana-pricing-api-openapi.yml
  format: yaml
  label: Dana Pricing API
  slug: dana-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-pricing-api-openapi.yml
- filename: dana-shipping-api-openapi.yml
  format: yaml
  label: Dana Shipping API
  slug: dana-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-shipping-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dana secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dana
provider_slug: dana
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/dana-aftermarket-api-openapi.yml
  type: apiKey
slug: dana-authentication
source_filename: dana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dana-aftermarket-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/dana-aftermarket-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/authentication/dana-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Aftermarket
- Auto Parts
- Drivetrain
- eCommerce
- Supply Chain
- Fortune 500
---
