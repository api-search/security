---
api_key_in:
- header
api_specs:
- filename: locations-openapi.json
  format: json
  label: Australia Post Locations API
  slug: locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/locations-openapi.json
- filename: delivery-partner-openapi.json
  format: json
  label: Australia Post Delivery Partner API
  slug: delivery-partner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/delivery-partner-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Australia Post Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australia Post secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Australia Post
provider_slug: australia-post
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: AUTH-KEY
  sources:
  - openapi/delivery-partner-openapi.json
  - openapi/locations-openapi.json
  type: apiKey
slug: australia-post-authentication
source_filename: australia-post-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/delivery-partner-openapi.json, openapi/locations-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: AUTH-KEY\n  sources:\n  - openapi/delivery-partner-openapi.json\n  - openapi/locations-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/authentication/australia-post-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Address Validation
- Click and Collect
- Delivery
- E-Commerce
- Labels
- Locations
- Logistics
- Parcel Locker
- Postal
- Postage
- Shipping
- Tracking
---
