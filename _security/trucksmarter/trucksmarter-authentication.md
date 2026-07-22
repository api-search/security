---
api_key_in: []
api_specs:
- filename: trucksmarter-load-posting-openapi.yml
  format: yaml
  label: TruckSmarter Load Posting API
  slug: trucksmarter-load-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trucksmarter/refs/heads/main/openapi/trucksmarter-load-posting-openapi.yml
auth_types:
- http
description: Authentication profile for the TruckSmarter Load Posting API (partner API). The published documentation states that all endpoints require an API key passed via the Authorization header as a Bearer token. API keys are issued to partners; no self-serve key provisioning, OAuth, or OpenID Connect surface is published.
kind: authentication
layout: security
method: searched
name: Trucksmarter Authentication
name_suffix: Authentication
oauth_flows: []
overview: TruckSmarter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TruckSmarter
provider_slug: trucksmarter
scheme_count: 1
schemes:
- description: 'All endpoints require an API key passed via the Authorization header: Authorization: Bearer YOUR_API_KEY'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trucksmarter-load-posting-openapi.yml
  type: http
slug: trucksmarter-authentication
source_filename: trucksmarter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://trucksmarter.notion.site/TruckSmarter-API-Load-Posting-Documentation-2014aa4e9bc580fe80cfe87e18516dea\ndocs: https://trucksmarter.notion.site/TruckSmarter-API-Load-Posting-Documentation-2014aa4e9bc580fe80cfe87e18516dea\ndescription: >-\n  Authentication profile for the TruckSmarter Load Posting API (partner API).\n  The published documentation states that all endpoints require an API key\n  passed via the Authorization header as a Bearer token. API keys are issued\n  to partners; no self-serve key provisioning, OAuth, or OpenID Connect\n  surface is published.\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: 'All endpoints require an API key passed via the Authorization header: Authorization: Bearer YOUR_API_KEY'\n    sources:\n      - openapi/trucksmarter-load-posting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trucksmarter/refs/heads/main/authentication/trucksmarter-authentication.yml
summary_line: http · 1 scheme
tags:
- Trucking
- Freight
- Logistics
- Load Board
- Transportation
- Dispatch
- Fuel
- Factoring
---
