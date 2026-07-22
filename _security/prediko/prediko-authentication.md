---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Prediko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prediko secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prediko
provider_slug: prediko
scheme_count: 1
schemes:
- description: All API requests authenticate with a Prediko API key passed as an Authorization bearer token. Keys use the prefix pk_live_ and are created in the Prediko Dashboard under Settings > API Keys. A key is displayed only once at creation; lost keys must be recreated. Missing or invalid keys return 401.
  header: Authorization
  header_format: 'Authorization: Bearer pk_live_YOUR_API_KEY'
  key_prefix: pk_live_
  name: bearerApiKey
  provisioning: Prediko Dashboard > Settings > API Keys > Create API Key
  scheme: bearer
  sources:
  - https://api.prediko.io/docs/authentication/
  type: http
slug: prediko-authentication
source_filename: prediko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.prediko.io/docs/authentication/\ndocs: https://api.prediko.io/docs/authentication/\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    All API requests authenticate with a Prediko API key passed as an\n    Authorization bearer token. Keys use the prefix pk_live_ and are created in\n    the Prediko Dashboard under Settings > API Keys. A key is displayed only once\n    at creation; lost keys must be recreated. Missing or invalid keys return 401.\n  header: Authorization\n  header_format: 'Authorization: Bearer pk_live_YOUR_API_KEY'\n  key_prefix: pk_live_\n  provisioning: Prediko Dashboard > Settings > API Keys > Create API Key\n  sources:\n  - https://api.prediko.io/docs/authentication/\nnotes: >-\n  No OAuth2/OIDC flows are offered. Insufficient permissions on a valid key\n  return 403. No test-key (pk_test_)\
  \ prefix is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prediko/refs/heads/main/authentication/prediko-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Inventory Management
- Demand Forecasting
- Supply Chain
- Ecommerce
- Shopify
- Purchase Orders
- Retail
- AI
---
