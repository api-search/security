---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: My Real Trip Authentication
name_suffix: Authentication
oauth_flows: []
overview: My Real Trip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: My Real Trip
provider_slug: my-real-trip
scheme_count: 1
schemes:
- description: API key sent in the Authorization header using the Bearer scheme. Test keys are prefixed test_sk_ (per docs example). Missing header or a missing "Bearer " prefix returns 401; a valid key without resource permission returns 403.
  format: Bearer YOUR_API_KEY
  header: Authorization
  in: header
  name: bearerApiKey
  scheme: bearer
  sources:
  - https://docs.myrealtrip.com/#auth
  type: http
slug: my-real-trip-authentication
source_filename: my-real-trip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.myrealtrip.com/#auth\ndocs: https://docs.myrealtrip.com/#auth\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The MyRealTrip Partner API uses a static API key presented as an HTTP\n    Bearer token. There is no OAuth2/OIDC surface and no scope model. Keys are\n    issued from the Partner page (Open API menu, \"API Key 발급\") and are shown\n    only once at creation; re-issuing a key immediately expires the previous\n    one. Keys must be used server-side only.\nschemes:\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer YOUR_API_KEY'\n    sources: [https://docs.myrealtrip.com/#auth]\n    description: >-\n      API key sent in the Authorization header using the Bearer scheme. Test\n      keys are prefixed test_sk_ (per docs example). Missing header or a\n      missing \"Bearer\
  \ \" prefix returns 401; a valid key without resource\n      permission returns 403.\nkey_management:\n  issuance: Partner page -> Open API -> \"API Key 발급\"\n  visibility: full value shown only at creation, masked thereafter\n  rotation: re-issue creates a new key and auto-expires the previous key\n  transport: HTTPS only, TLS 1.2+\n  support: marketing_partner@myrealtrip.com\ntransport_security:\n  https_required: true\n  min_tls: '1.2'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/my-real-trip/refs/heads/main/authentication/my-real-trip-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Travel
- Tourism
- Flights
- Accommodation
- Tours and Activities
- Affiliate
- MCP
- South Korea
---
