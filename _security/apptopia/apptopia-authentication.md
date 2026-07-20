---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Apptopia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apptopia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apptopia
provider_slug: apptopia
scheme_count: 1
schemes:
- bearer_format: JWT
  header: Authorization
  in: header
  name: jwtBearer
  scheme: bearer
  sources:
  - https://dev.apptopia.com/
  token_endpoint: https://integrations.apptopia.com/api/login
  token_lifetime: 1209600
  type: http
slug: apptopia-authentication
source_filename: apptopia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://dev.apptopia.com/\ndocs: https://dev.apptopia.com/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  Apptopia's Data API uses JSON Web Token (JWT) bearer authentication. A client\n  POSTs credentials to /api/login and receives a JWT, which is sent verbatim in\n  the Authorization header on every subsequent request. Tokens expire after two\n  weeks by default and must be refreshed by logging in again. There is no OAuth,\n  no API-key parameter, and no per-request scope surface documented.\nschemes:\n  - name: jwtBearer\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    header: Authorization\n    token_endpoint: https://integrations.apptopia.com/api/login\n    token_lifetime: 1209600  # ~2 weeks in seconds\n    sources: [https://dev.apptopia.com/]\nlogin:\n  method: POST\n  path: /api/login\n  base_url: https://integrations.apptopia.com\n\
  \  credentials: [username, password]\n  returns: JWT (sent as the Authorization header value on subsequent requests)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptopia/refs/heads/main/authentication/apptopia-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Mobile
- App Store Intelligence
- Market Intelligence
- Alternative Data
- Analytics
- Consumer Insights
- Advertising
---
