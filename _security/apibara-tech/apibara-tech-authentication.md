---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: apibara-tech-openapi.json
  format: json
  label: Vehicle Auction Data API
  slug: vehicle-auction-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-openapi.json
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
