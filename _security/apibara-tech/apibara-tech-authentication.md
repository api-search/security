---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: apibara-tech-filters-api-openapi.yml
  format: yaml
  label: Apibara.tech Filters API
  slug: apibara-tech-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-filters-api-openapi.yml
- filename: apibara-tech-image-proxy-api-openapi.yml
  format: yaml
  label: Apibara.tech Image Proxy API
  slug: apibara-tech-image-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-image-proxy-api-openapi.yml
- filename: apibara-tech-locations-api-openapi.yml
  format: yaml
  label: Apibara.tech Locations API
  slug: apibara-tech-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-locations-api-openapi.yml
- filename: apibara-tech-related-vehicles-api-openapi.yml
  format: yaml
  label: Apibara.tech Related Vehicles API
  slug: apibara-tech-related-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-related-vehicles-api-openapi.yml
- filename: apibara-tech-shipping-api-openapi.yml
  format: yaml
  label: Apibara.tech Shipping API
  slug: apibara-tech-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-shipping-api-openapi.yml
- filename: apibara-tech-url-tools-api-openapi.yml
  format: yaml
  label: Apibara.tech URL Tools API
  slug: apibara-tech-url-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-url-tools-api-openapi.yml
- filename: apibara-tech-usage-api-openapi.yml
  format: yaml
  label: Apibara.tech Usage API
  slug: apibara-tech-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-usage-api-openapi.yml
- filename: apibara-tech-vehicle-history-api-openapi.yml
  format: yaml
  label: Apibara.tech Vehicle History API
  slug: apibara-tech-vehicle-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-vehicle-history-api-openapi.yml
- filename: apibara-tech-vehicles-api-openapi.yml
  format: yaml
  label: Apibara.tech Vehicles API
  slug: apibara-tech-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-vehicles-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Apibara Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apibara.tech secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apibara.tech
provider_slug: apibara-tech
scheme_count: 1
schemes:
- description: Apibara API key.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/apibara-tech-openapi.json
  type: apiKey
slug: apibara-tech-authentication
source_filename: apibara-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: derived\nsource: openapi/apibara-tech-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Apibara API key.\n  sources:\n  - openapi/apibara-tech-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/authentication/apibara-tech-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automotive
- vehicle-auction-data
- Copart
- IAAI
- vin-history
- Marketplace
- REST API
- Vehicle Auctions
- Salvage Auctions
- VIN Data
- Used-Car Marketplace Data
- Data Infrastructure
- Data as a Service
- REST
- JSON:API
- MCP
- Agent-Native
---
