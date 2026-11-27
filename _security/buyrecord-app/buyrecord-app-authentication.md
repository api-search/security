---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buyrecord-app-keys-api-openapi.yml
  format: yaml
  label: BuyRecord Keys API
  slug: buyrecord-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-keys-api-openapi.yml
- filename: buyrecord-app-merchants-api-openapi.yml
  format: yaml
  label: BuyRecord Merchants API
  slug: buyrecord-app-merchants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-merchants-api-openapi.yml
- filename: buyrecord-app-outcomes-api-openapi.yml
  format: yaml
  label: BuyRecord Outcomes API
  slug: buyrecord-app-outcomes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-outcomes-api-openapi.yml
- filename: buyrecord-app-products-api-openapi.yml
  format: yaml
  label: BuyRecord Products API
  slug: buyrecord-app-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-products-api-openapi.yml
- filename: buyrecord-app-stays-api-openapi.yml
  format: yaml
  label: BuyRecord Stays API
  slug: buyrecord-app-stays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-stays-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: BuyRecord Authentication
name_suffix: Authentication
oauth_flows: []
overview: BuyRecord secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BuyRecord
provider_slug: buyrecord-app
scheme_count: 1
schemes:
- description: API key (br_live_...). Required for writing.
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/buyrecord-app-openapi.json
  type: http
slug: buyrecord-app-authentication
source_filename: buyrecord-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/buyrecord-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: API key (br_live_...). Required for writing.\n  sources:\n  - openapi/buyrecord-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/buyrecord-app/authentication/buyrecord-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- E-Commerce
- Data
- Shopping
- Analytics
---
