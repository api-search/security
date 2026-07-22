---
api_key_in:
- header
api_specs:
- filename: packlink-openapi.yml
  format: yaml
  label: Packlink PRO Shipping API
  slug: packlink-pro-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packlink/refs/heads/main/openapi/packlink-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Packlink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Packlink secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Packlink
provider_slug: packlink
scheme_count: 1
schemes:
- description: Packlink PRO API key passed in the Authorization header. Obtain the key from the Packlink PRO dashboard under Settings > Packlink PRO API.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/packlink-openapi.yml
  type: apiKey
slug: packlink-authentication
source_filename: packlink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/packlink-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Packlink PRO API key passed in the Authorization header. Obtain the key from\n    the Packlink PRO dashboard under Settings > Packlink PRO API.\n  sources:\n  - openapi/packlink-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packlink/refs/heads/main/authentication/packlink-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ecommerce
- Shipping
- Logistics
- Parcel Delivery
- Carriers
- Fulfillment
---
