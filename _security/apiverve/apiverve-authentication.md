---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: apiverve-openapi.yaml
  format: yaml
  label: APIVerve REST API
  slug: apiverve-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiverve/refs/heads/main/openapi/apiverve-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Apiverve Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIVerve secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIVerve
provider_slug: apiverve
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/apiverve-openapi.yaml
  type: apiKey
slug: apiverve-authentication
source_filename: apiverve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: derived\nsource: openapi/apiverve-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/apiverve-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiverve/refs/heads/main/authentication/apiverve-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Marketplace
- REST
- JSON
- GraphQL
- OpenAPI
- Postman
- MCP
- llms-txt
- agent-native
- APIKeys
- IP Geolocation
- DNS
- WHOIS
- SSL
- Email Validation
- Phone Validation
- Exchange Rates
- metals prices
- Weather
- Geocoding
- Text Processing
- Developer Tools
---
