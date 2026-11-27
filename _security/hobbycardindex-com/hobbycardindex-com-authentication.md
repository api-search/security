---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hobbycardindex-com-bulk-files-api-openapi.yml
  format: yaml
  label: Hobby Card Index bulk files API
  slug: hobbycardindex-com-bulk-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-bulk-files-api-openapi.yml
- filename: hobbycardindex-com-catalog-api-openapi.yml
  format: yaml
  label: Hobby Card Index Catalog API
  slug: hobbycardindex-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-catalog-api-openapi.yml
- filename: hobbycardindex-com-collection-api-openapi.yml
  format: yaml
  label: Hobby Card Index Collection API
  slug: hobbycardindex-com-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-collection-api-openapi.yml
- filename: hobbycardindex-com-market-api-openapi.yml
  format: yaml
  label: Hobby Card Index Market API
  slug: hobbycardindex-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-market-api-openapi.yml
- filename: hobbycardindex-com-mcp-api-openapi.yml
  format: yaml
  label: Hobby Card Index MCP API
  slug: hobbycardindex-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-mcp-api-openapi.yml
- filename: hobbycardindex-com-prices-api-openapi.yml
  format: yaml
  label: Hobby Card Index Prices API
  slug: hobbycardindex-com-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-prices-api-openapi.yml
- filename: hobbycardindex-com-sales-api-openapi.yml
  format: yaml
  label: Hobby Card Index Sales API
  slug: hobbycardindex-com-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-sales-api-openapi.yml
- filename: hobbycardindex-com-scan-api-openapi.yml
  format: yaml
  label: Hobby Card Index Scan API
  slug: hobbycardindex-com-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-scan-api-openapi.yml
- filename: hobbycardindex-com-slabs-and-certs-api-openapi.yml
  format: yaml
  label: Hobby Card Index slabs and certs API
  slug: hobbycardindex-com-slabs-and-certs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-slabs-and-certs-api-openapi.yml
- filename: hobbycardindex-com-usage-api-openapi.yml
  format: yaml
  label: Hobby Card Index Usage API
  slug: hobbycardindex-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-usage-api-openapi.yml
- filename: hobbycardindex-com-watch-list-and-webhooks-api-openapi.yml
  format: yaml
  label: Hobby Card Index watch list and webhooks API
  slug: hobbycardindex-com-watch-list-and-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hobbycardindex-com/openapi/hobbycardindex-com-watch-list-and-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hobby Card Index Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hobby Card Index secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hobby Card Index
provider_slug: hobbycardindex-com
scheme_count: 1
schemes:
- description: 'Your HobbyCardIndex API key (hci_live_...). `Authorization: Bearer <key>` is accepted too. Keys: https://hobbycardindex.com/developers.'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/hobbycardindex-com-openapi.json
  type: apiKey
slug: hobbycardindex-com-authentication
source_filename: hobbycardindex-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hobbycardindex-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Your HobbyCardIndex API key (hci_live_...). `Authorization: Bearer <key>` is\n    accepted too. Keys: https://hobbycardindex.com/developers.'\n  sources:\n  - openapi/hobbycardindex-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hobbycardindex-com/authentication/hobbycardindex-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cards
- Pricing
- Sports
- Collectibles
- Trading
---
