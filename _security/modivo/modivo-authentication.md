---
api_key_in:
- header
api_specs:
- filename: modivo-commerce-rest-api-openapi.yml
  format: yaml
  label: MODIVO Commerce REST API
  slug: modivo-commerce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modivo/refs/heads/main/openapi/modivo-commerce-rest-api-openapi.yml
- filename: modivo-eobuwie-commerce-rest-api-openapi.yml
  format: yaml
  label: eobuwie Commerce REST API
  slug: eobuwie-commerce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modivo/refs/heads/main/openapi/modivo-eobuwie-commerce-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Modivo Authentication
name_suffix: Authentication
oauth_flows: []
overview: MODIVO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MODIVO
provider_slug: modivo
scheme_count: 1
schemes:
- description: Magento integration/customer bearer token supplied in the Authorization header (Bearer <token>).
  in: header
  name: api_key
  parameter: api_key
  sources:
  - openapi/modivo-commerce-rest-api-openapi.yml
  type: apiKey
slug: modivo-authentication
source_filename: modivo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/modivo-commerce-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: Magento integration/customer bearer token supplied in the Authorization header\n    (Bearer <token>).\n  sources:\n  - openapi/modivo-commerce-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modivo/refs/heads/main/authentication/modivo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Fashion
- E-Commerce
- Retail
- Marketplace
- Retail Media
- Commerce
- Checkout
- Catalog
- GraphQL
- Adobe Commerce
- Magento
- Poland
- Central Europe
---
