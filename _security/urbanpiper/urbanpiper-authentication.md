---
api_key_in:
- header
api_specs:
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Catalog & Menu API
  slug: catalog-menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Stores & Locations API
  slug: stores-locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Item Availability API
  slug: item-availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Urbanpiper Authentication
name_suffix: Authentication
oauth_flows: []
overview: UrbanPiper secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UrbanPiper
provider_slug: urbanpiper
scheme_count: 1
schemes:
- description: 'Static API key authentication. Pass the header as `Authorization: apikey <api_username>:<api_key>`. Multi-brand requests must also include the `X-UPR-Biz-Id` header identifying the business/brand.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/urbanpiper-openapi.yml
  type: apiKey
slug: urbanpiper-authentication
source_filename: urbanpiper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/urbanpiper-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Static API key authentication. Pass the header as `Authorization: apikey <api_username>:<api_key>`.\n    Multi-brand requests must also include the `X-UPR-Biz-Id` header identifying the business/brand.'\n  sources:\n  - openapi/urbanpiper-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/authentication/urbanpiper-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurants
- Food Delivery
- Ordering
- POS
- Aggregators
- Commerce
---
