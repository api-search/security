---
api_key_in:
- header
api_specs:
- filename: rekki-catalog-api-openapi.yml
  format: yaml
  label: REKKI catalog API
  slug: rekki-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/openapi/rekki-catalog-api-openapi.yml
- filename: rekki-connect-customers-api-openapi.yml
  format: yaml
  label: REKKI connect_customers API
  slug: rekki-connect-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/openapi/rekki-connect-customers-api-openapi.yml
- filename: rekki-general-api-openapi.yml
  format: yaml
  label: REKKI general API
  slug: rekki-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/openapi/rekki-general-api-openapi.yml
- filename: rekki-order-guide-api-openapi.yml
  format: yaml
  label: REKKI order-guide API
  slug: rekki-order-guide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/openapi/rekki-order-guide-api-openapi.yml
- filename: rekki-orders-api-openapi.yml
  format: yaml
  label: REKKI orders API
  slug: rekki-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/openapi/rekki-orders-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rekki Authentication
name_suffix: Authentication
oauth_flows: []
overview: REKKI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: REKKI
provider_slug: rekki
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/rekki-supplier-api-openapi-original.json
  type: apiKey
slug: rekki-authentication
source_filename: rekki-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/rekki-supplier-api-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/rekki-supplier-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/authentication/rekki-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Food
- Wholesale
- Ordering
- Restaurant
- Supply Chain
- Catalog
- Order
- E-Commerce
---
