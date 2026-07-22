---
api_key_in:
- header
api_specs:
- filename: maison-safqa-holdings-limited-openapi-original.yml
  format: yaml
  label: Maison Safqa Brand Developer API
  slug: maison-safqa-brand-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maison-safqa-holdings-limited/refs/heads/main/openapi/maison-safqa-holdings-limited-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Maison Safqa Holdings Limited Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maison Safqa Holdings Limited secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Maison Safqa Holdings Limited
provider_slug: maison-safqa-holdings-limited
scheme_count: 1
schemes:
- description: API key for authentication. Use 'ms_test_...' keys for development/testing and 'ms_live_...' keys for production. Keys are environment-specific and will only work in their respective environments.
  in: header
  name: ApiKeyAuth
  parameter: X-MaisonSafqa-Api-Key
  sources:
  - openapi/maison-safqa-holdings-limited-openapi-original.yml
  type: apiKey
slug: maison-safqa-holdings-limited-authentication
source_filename: maison-safqa-holdings-limited-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/maison-safqa-holdings-limited-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-MaisonSafqa-Api-Key\n  description: API key for authentication. Use 'ms_test_...' keys for development/testing and\n    'ms_live_...' keys for production. Keys are environment-specific and will only work in their\n    respective environments.\n  sources:\n  - openapi/maison-safqa-holdings-limited-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maison-safqa-holdings-limited/refs/heads/main/authentication/maison-safqa-holdings-limited-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Retail
- E-commerce
- Luxury
- Marketplace
- Product Catalog
- Inventory Management
- Shopify
---
