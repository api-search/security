---
api_key_in: []
api_specs:
- filename: nar-m1-gateway-external-openapi.json
  format: json
  label: REALTORS M1 Gateway External API
  slug: nar-m1-gateway-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nar/refs/heads/main/openapi/nar-m1-gateway-external-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nar Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Association of REALTORS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: National Association of REALTORS
provider_slug: nar
scheme_count: 1
schemes:
- description: Basic Authorization header using user and password
  name: basic
  scheme: basic
  sources:
  - openapi/nar-m1-gateway-external-openapi.json
  type: http
slug: nar-authentication
source_filename: nar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/nar-m1-gateway-external-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: Basic Authorization header using user and password\n  sources:\n  - openapi/nar-m1-gateway-external-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nar/refs/heads/main/authentication/nar-authentication.yml
summary_line: http · 1 scheme
tags:
- Real Estate
- United States
- Industry Body
- MLS
- RESO
- Standards
- Membership
- Property Listings
- IDX
- PropTech
---
