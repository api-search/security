---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Chartbeat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chartbeat secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chartbeat
provider_slug: chartbeat
scheme_count: 2
schemes:
- applies_to:
  - Real-Time API (https://api.chartbeat.com/live/)
  - Historical / Advanced Queries API (https://api.chartbeat.com/query/v2/)
  - Headline Testing API
  - Conversion API
  - Data Lab API
  description: Chartbeat API key passed in the HTTP request header as 'X-CB-AK'. The key is generated and managed in Chartbeat account settings. This is the current documented authentication method for the Real-Time, Historical (Advanced Queries), Headline Testing, Conversion, and Data Lab APIs.
  in: header
  name: X-CB-AK
  parameter: X-CB-AK
  type: apiKey
- description: Legacy API-key delivery as an 'apikey' query-string parameter, still shown in older Help Center examples for the Advanced Queries API. Header-based X-CB-AK is the preferred/current method.
  in: query
  name: apikey
  parameter: apikey
  type: apiKey
slug: chartbeat-authentication
source_filename: chartbeat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.chartbeat.com/cbp/api/real-time-apis/getting-started-with-our-real-time-api\ndocs: https://help.chartbeat.com/hc/en-us/articles/360036657754-Create-and-manage-API-keys\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\nschemes:\n  - name: X-CB-AK\n    type: apiKey\n    in: header\n    parameter: X-CB-AK\n    description: >-\n      Chartbeat API key passed in the HTTP request header as 'X-CB-AK'. The key\n      is generated and managed in Chartbeat account settings. This is the\n      current documented authentication method for the Real-Time, Historical\n      (Advanced Queries), Headline Testing, Conversion, and Data Lab APIs.\n    applies_to:\n      - Real-Time API (https://api.chartbeat.com/live/)\n      - Historical / Advanced Queries API (https://api.chartbeat.com/query/v2/)\n      - Headline Testing API\n      - Conversion API\n      - Data Lab API\n  - name: apikey\n    type: apiKey\n    in: query\n\
  \    parameter: apikey\n    description: >-\n      Legacy API-key delivery as an 'apikey' query-string parameter, still shown\n      in older Help Center examples for the Advanced Queries API. Header-based\n      X-CB-AK is the preferred/current method.\nnotes:\n  - No OAuth2 / OpenID Connect surface is documented; there is no scope model.\n  - API keys are account-scoped and gate access per site/host and per plan tier\n    (Advanced Queries and some feature APIs are Premium add-ons).\n  - API usage is governed by Chartbeat's API terms (https://chartbeat.com/apiterms/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chartbeat/refs/heads/main/authentication/chartbeat-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- SaaS
- Analytics
- Content Analytics
- Real-Time Analytics
- Audience Engagement
- Publishing
- Media
- Web Analytics
- Video Analytics
---
