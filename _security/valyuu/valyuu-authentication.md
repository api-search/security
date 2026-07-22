---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Valyuu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Valyuu secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Valyuu
provider_slug: valyuu
scheme_count: 1
schemes:
- description: Partner-issued API key sent as the X-Api-Key request header on all Valyuu Partner API v1 calls.
  in: header
  name: X-Api-Key
  parameter: X-Api-Key
  sources:
  - https://github.com/Valyuu/partner-api-frontend-demo/blob/main/src/queries/query-categories.ts
  - https://github.com/Valyuu/partner-api-frontend-demo/blob/main/README.md
  type: apiKey
slug: valyuu-authentication
source_filename: valyuu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: https://github.com/Valyuu/partner-api-frontend-demo\nnotes: No OpenAPI is harvested in this repo (the documented Swagger endpoint\n  https://api-staging.valyuu.tech/partner/swagger-json returned HTTP 522 on\n  2026-07-21). This profile is derived from Valyuu's public Partner API frontend\n  demo, whose API client sends an X-Api-Key header on every request and whose\n  README documents an API_AUTH_KEY environment variable (a partner-issued key;\n  a demo key is published in the repository README).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Partner-issued API key sent as the X-Api-Key request header on all\n    Valyuu Partner API v1 calls.\n  sources:\n  - https://github.com/Valyuu/partner-api-frontend-demo/blob/main/src/queries/query-categories.ts\n  - https://github.com/Valyuu/partner-api-frontend-demo/blob/main/README.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valyuu/refs/heads/main/authentication/valyuu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Recommerce
- Trade-In
- Circular Economy
- Consumer Electronics
- Sustainability
- eCommerce
---
