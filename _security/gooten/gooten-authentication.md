---
api_key_in:
- query
api_specs:
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Products API
  slug: gooten-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Orders API
  slug: gooten-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Shipping API
  slug: gooten-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Print Assets API
  slug: gooten-print-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gooten Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gooten secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gooten
provider_slug: gooten
scheme_count: 1
schemes:
- description: Public RecipeID from the Gooten Admin, required on every request. Order-writing and billing endpoints additionally require a private PartnerBillingKey query parameter (URL-encoded).
  in: query
  name: recipeId
  parameter: RecipeID
  sources:
  - openapi/gooten-openapi.yml
  type: apiKey
slug: gooten-authentication
source_filename: gooten-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gooten-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: recipeId\n  type: apiKey\n  in: query\n  parameter: RecipeID\n  description: Public RecipeID from the Gooten Admin, required on every request. Order-writing\n    and billing endpoints additionally require a private PartnerBillingKey query parameter (URL-encoded).\n  sources:\n  - openapi/gooten-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/authentication/gooten-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Print on Demand
- Fulfillment
- Manufacturing
- Ecommerce
- Dropshipping
- Custom Products
---
