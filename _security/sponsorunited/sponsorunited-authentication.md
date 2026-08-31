---
api_key_in:
- header
api_specs:
- filename: sponsorunited-api-openapi.json
  format: json
  label: SponsorUnited API
  slug: sponsorunited-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sponsorunited/refs/heads/main/openapi/sponsorunited-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sponsorunited Authentication
name_suffix: Authentication
oauth_flows: []
overview: SponsorUnited secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SponsorUnited
provider_slug: sponsorunited
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sponsorunited-api-openapi.json
  type: http
- description: 'Service API key for external services (ai-api, chat-api). Generate with: php artisan su:api-token:generate'
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/sponsorunited-api-openapi.json
  type: apiKey
slug: sponsorunited-authentication
source_filename: sponsorunited-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/sponsorunited-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/sponsorunited-api-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Service API key for external services (ai-api, chat-api). Generate with: php\n    artisan su:api-token:generate'\n  sources:\n  - openapi/sponsorunited-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sponsorunited/refs/heads/main/authentication/sponsorunited-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Sponsorship
- Sports
- Entertainment
- Marketing
- Advertising
- Media
- Data
- Analytics
- Market Intelligence
- Software-as-a-Service
- Partnerships
---
