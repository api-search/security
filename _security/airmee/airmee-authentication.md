---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: airmee-integration-api-openapi.yml
  format: yaml
  label: Airmee Integration API
  slug: airmee-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airmee/refs/heads/main/openapi/airmee-integration-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Airmee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airmee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airmee
provider_slug: airmee
scheme_count: 1
schemes:
- description: Pickup place's long-lived JWT issued by Airmee, sent as the raw value of the Authorization header (the published curl examples use `Authorization:<YOUR_JWT>` with no scheme prefix).
  in: header
  name: jwtAuth
  parameter: Authorization
  sources:
  - openapi/airmee-integration-api-openapi.yml
  type: apiKey
slug: airmee-authentication
source_filename: airmee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/airmee-integration-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: jwtAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Pickup place's long-lived JWT issued by Airmee, sent as the raw value of the\n    Authorization header (the published curl examples use `Authorization:<YOUR_JWT>` with no\n    scheme prefix).\n  sources:\n  - openapi/airmee-integration-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airmee/refs/heads/main/authentication/airmee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Logistics
- Last Mile Delivery
- Shipping
- Parcel Delivery
- Parcel Lockers
- Returns
- E-Commerce
- Same-Day Delivery
- Sweden
- Carrier
---
