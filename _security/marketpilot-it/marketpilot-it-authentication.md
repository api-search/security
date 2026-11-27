---
anonymous_access: false
api_key_in: []
api_specs:
- filename: marketpilot-it-orders-api-openapi.yml
  format: yaml
  label: MarketPilot Orders API
  slug: marketpilot-it-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketpilot-it/openapi/marketpilot-it-orders-api-openapi.yml
- filename: marketpilot-it-point-api-openapi.yml
  format: yaml
  label: MarketPilot Point API
  slug: marketpilot-it-point-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketpilot-it/openapi/marketpilot-it-point-api-openapi.yml
- filename: marketpilot-it-press-api-openapi.yml
  format: yaml
  label: MarketPilot Press API
  slug: marketpilot-it-press-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketpilot-it/openapi/marketpilot-it-press-api-openapi.yml
- filename: marketpilot-it-products-api-openapi.yml
  format: yaml
  label: MarketPilot Products API
  slug: marketpilot-it-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketpilot-it/openapi/marketpilot-it-products-api-openapi.yml
- filename: marketpilot-it-public-api-openapi.yml
  format: yaml
  label: MarketPilot Public API
  slug: marketpilot-it-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketpilot-it/openapi/marketpilot-it-public-api-openapi.yml
- filename: marketpilot-it-search-places-api-openapi.yml
  format: yaml
  label: MarketPilot Search Places API
  slug: marketpilot-it-search-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketpilot-it/openapi/marketpilot-it-search-places-api-openapi.yml
- filename: marketpilot-it-support-api-openapi.yml
  format: yaml
  label: MarketPilot Support API
  slug: marketpilot-it-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketpilot-it/openapi/marketpilot-it-support-api-openapi.yml
- filename: marketpilot-it-tools-api-openapi.yml
  format: yaml
  label: MarketPilot Tools API
  slug: marketpilot-it-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketpilot-it/openapi/marketpilot-it-tools-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MarketPilot Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarketPilot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MarketPilot
provider_slug: marketpilot-it
scheme_count: 1
schemes:
- description: www.marketpilot.it/developer/api-keys 에서 발급한 mk_ 키
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/marketpilot-it-ai-openapi.json
  type: http
slug: marketpilot-it-authentication
source_filename: marketpilot-it-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/marketpilot-it-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: www.marketpilot.it/developer/api-keys 에서 발급한 mk_ 키\n  sources:\n  - openapi/marketpilot-it-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/marketpilot-it/authentication/marketpilot-it-authentication.yml
summary_line: http · 1 scheme
tags:
- Marketing
- Artificial Intelligence
- E-Commerce
- Small Business
- South Korea
---
