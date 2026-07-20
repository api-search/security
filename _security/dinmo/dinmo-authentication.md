---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Dinmo Authentication
name_suffix: Authentication
oauth_flows: []
overview: DinMo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DinMo
provider_slug: dinmo
scheme_count: 1
schemes:
- description: 'A DinMo Personalization API key is sent in the HTTP Authorization header as a Bearer token (Authorization: Bearer <API_KEY>). Keys are generated in the DinMo app and scoped to a workspace''s exposed model records. A missing or invalid key returns 401.'
  format: Bearer <API_KEY>
  location: header
  name: PersonalizationApiKey
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.dinmo.io/customer-hub/profiles-api/api-reference
  type: http
slug: dinmo-authentication
source_filename: dinmo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.dinmo.io/customer-hub/profiles-api/api-reference\ndocs: https://docs.dinmo.io/customer-hub/profiles-api/api-reference\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  http_schemes:\n  - bearer\nschemes:\n- name: PersonalizationApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    A DinMo Personalization API key is sent in the HTTP Authorization header as a\n    Bearer token (Authorization: Bearer <API_KEY>). Keys are generated in the DinMo\n    app and scoped to a workspace's exposed model records. A missing or invalid key\n    returns 401.\n  location: header\n  parameter: Authorization\n  format: Bearer <API_KEY>\n  sources:\n  - https://docs.dinmo.io/customer-hub/profiles-api/api-reference\nnotes: >-\n  Platform access (data sources, destinations, segments) is configured through the\n  DinMo web app; the documented programmatic surface is the Personalization API,\n  which uses\
  \ Bearer [example key] authentication. No OAuth2 or OpenID Connect flow is\n  documented for the public API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dinmo/refs/heads/main/authentication/dinmo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Customer Data Platform
- CDP
- Reverse ETL
- Data Activation
- Data Warehouse
- Audience Segmentation
- Marketing
- Personalization
- MarTech
---
