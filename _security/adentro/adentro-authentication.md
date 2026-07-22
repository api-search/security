---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Adentro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adentro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adentro
provider_slug: adentro
scheme_count: 1
schemes:
- description: Customers are issued an Adentro API Token that must be passed via the Authorization header on all API requests. Tokens are issued manually by Adentro and their expiration/rotation policy is managed by Adentro (contact the Adentro account/engineering team to obtain one). Applies to the Contacts API and the Location & Scanning API (V2 and V3).
  in: header
  name: adentroToken
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.fishbowl.com/knowledge/adentro-wifi
  - https://support.adentro.com/s/article/V2-V3-Location-Scanning-Migration
  type: http
slug: adentro-authentication
source_filename: adentro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://support.adentro.com/s/article/V2-V3-Location-Scanning-Migration\ndocs: https://support.adentro.com/s/\nnote: >-\n  Adentro (formerly Zenreach) does not publish a public OpenAPI spec or self-serve\n  developer portal. API access is partner/customer-gated. These auth details are\n  captured verbatim from Adentro support articles and from published partner\n  integration guides (Fishbowl GRM, Alpine IQ) that document connecting to the\n  Adentro Contacts API and Location & Scanning API.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: adentroToken\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    Customers are issued an Adentro API Token that must be passed via the\n    Authorization header on all API requests. Tokens are issued manually by\n    Adentro and their expiration/rotation policy is managed by Adentro (contact\n    the Adentro\
  \ account/engineering team to obtain one). Applies to the Contacts\n    API and the Location & Scanning API (V2 and V3).\n  sources:\n  - https://docs.fishbowl.com/knowledge/adentro-wifi\n  - https://support.adentro.com/s/article/V2-V3-Location-Scanning-Migration\napis:\n- name: Contacts API\n  auth: adentroToken\n  identifiers:\n    location_id: >-\n      Per-location scoping via Adentro Location IDs (the `business={id}` value in\n      the Adentro dashboard URL). Requests are scoped to the customer's locations.\n- name: Location & Scanning API\n  auth: adentroToken\n  versions:\n  - v2\n  - v3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adentro/refs/heads/main/authentication/adentro-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Apps
- WiFi Marketing
- Customer Intelligence
- Location Analytics
- Retail
- Marketing Attribution
- Guest WiFi
---
