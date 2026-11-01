---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: shelfatlas-com-chains-api-openapi.yml
  format: yaml
  label: shelfatlas-com Chains API
  slug: shelfatlas-com-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-chains-api-openapi.yml
- filename: shelfatlas-com-mcp-api-openapi.yml
  format: yaml
  label: shelfatlas-com MCP API
  slug: shelfatlas-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-mcp-api-openapi.yml
- filename: shelfatlas-com-observations-api-openapi.yml
  format: yaml
  label: shelfatlas-com Observations API
  slug: shelfatlas-com-observations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-observations-api-openapi.yml
- filename: shelfatlas-com-observedprices-api-openapi.yml
  format: yaml
  label: shelfatlas-com Observed Prices API
  slug: shelfatlas-com-observedprices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-observedprices-api-openapi.yml
- filename: shelfatlas-com-offers-api-openapi.yml
  format: yaml
  label: shelfatlas-com Offers API
  slug: shelfatlas-com-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-offers-api-openapi.yml
- filename: shelfatlas-com-price-history-api-openapi.yml
  format: yaml
  label: shelfatlas-com Price history API
  slug: shelfatlas-com-price-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-price-history-api-openapi.yml
- filename: shelfatlas-com-products-api-openapi.yml
  format: yaml
  label: shelfatlas-com Products API
  slug: shelfatlas-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-products-api-openapi.yml
- filename: shelfatlas-com-seoterms-api-openapi.yml
  format: yaml
  label: shelfatlas-com Seo Terms API
  slug: shelfatlas-com-seoterms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-seoterms-api-openapi.yml
- filename: shelfatlas-com-stats-api-openapi.yml
  format: yaml
  label: shelfatlas-com Stats API
  slug: shelfatlas-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-stats-api-openapi.yml
- filename: shelfatlas-com-stores-api-openapi.yml
  format: yaml
  label: shelfatlas-com Stores API
  slug: shelfatlas-com-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-stores-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Shelfatlas Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: shelfatlas-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: shelfatlas-com
provider_slug: shelfatlas-com
scheme_count: 2
schemes:
- description: 'A ShelfAtlas API key: `Authorization: Bearer sa_live_<key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/shelfatlas-com-openapi.json
  type: http
- description: 'Anonymous per-device identity for POST /api/v1/observations: a UUID the client generates and keeps locally. Any UUID version is accepted — the check is purely the 8-4-4-4-12 hex-digit shape.'
  in: header
  name: deviceTokenAuth
  parameter: X-Device-Token
  sources:
  - openapi/shelfatlas-com-openapi.json
  type: apiKey
slug: shelfatlas-com-authentication
source_filename: shelfatlas-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/shelfatlas-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A ShelfAtlas API key: `Authorization: Bearer sa_live_<key>`.'\n  sources:\n  - openapi/shelfatlas-com-openapi.json\n- name: deviceTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Device-Token\n  description: 'Anonymous per-device identity for POST /api/v1/observations: a UUID the client\n    generates and keeps locally. Any UUID version is accepted — the check is purely the 8-4-4-4-12\n    hex-digit shape.'\n  sources:\n  - openapi/shelfatlas-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/shelfatlas-com/authentication/shelfatlas-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Grocery
- API
- Denmark
- Retail
---
