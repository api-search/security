---
api_key_in: []
api_specs:
- filename: netography-openapi.yml
  format: yaml
  label: Netography (Vectra Fusion) API
  slug: netography-vectra-fusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netography/refs/heads/main/openapi/netography-openapi.yml
auth_types:
- http-bearer-jwt
- api-key-derived
description: ''
kind: authentication
layout: security
method: searched
name: Netography Authentication
name_suffix: Authentication
oauth_flows: []
overview: Netography secures its APIs with http-bearer-jwt and api-key-derived across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Netography
provider_slug: netography
scheme_count: 3
schemes:
- detail: Create a NETOSECRET API key in the Fusion Portal (Settings > User Management > API Keys). The netosecret encodes appkey/appname/shortname/sharedsecret + API URL. Sign a JWT request token with the shared secret and POST it as the `jwt` field to /api/v1/auth/token; the response access_token is the bearer token.
  kind: api-key -> JWT bearer
  name: apiKeyJwt
  token_endpoint: https://api.netography.com/api/v1/auth/token
- detail: POST username/password (x-www-form-urlencoded) to obtain an access_token.
  kind: password -> JWT bearer
  name: userCredentials
  token_endpoint: https://api.netography.com/api/auth/bearer/token
- detail: POST a refresh_token to obtain a new access_token.
  kind: refresh -> JWT bearer
  name: refreshToken
  token_endpoint: https://api.netography.com/api/auth/bearer/refresh
slug: netography-authentication
source_filename: netography-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.fusion.vectra.ai/api-reference/netography-apis/authentication.md\ndocs: https://docs.fusion.vectra.ai/api-reference/create-a-netography-api-key.md\nsummary:\n  types:\n  - http-bearer-jwt\n  - api-key-derived\n  token_type: bearer\n  token_format: JWT\nmodel: Netography Fusion authenticates all API calls with a JWT bearer access_token. There is no static\n  API key sent on each request; instead a short-lived bearer token is minted, then sent as the Authorization\n  header.\nschemes:\n- name: apiKeyJwt\n  kind: api-key -> JWT bearer\n  token_endpoint: https://api.netography.com/api/v1/auth/token\n  detail: Create a NETOSECRET API key in the Fusion Portal (Settings > User Management > API Keys). The\n    netosecret encodes appkey/appname/shortname/sharedsecret + API URL. Sign a JWT request token with\n    the shared secret and POST it as the `jwt` field to /api/v1/auth/token; the response access_token\n    is the\
  \ bearer token.\n- name: userCredentials\n  kind: password -> JWT bearer\n  token_endpoint: https://api.netography.com/api/auth/bearer/token\n  detail: POST username/password (x-www-form-urlencoded) to obtain an access_token.\n- name: refreshToken\n  kind: refresh -> JWT bearer\n  token_endpoint: https://api.netography.com/api/auth/bearer/refresh\n  detail: POST a refresh_token to obtain a new access_token.\nusage: 'Authorization: Bearer <access_token>'\nrecipes: https://docs.fusion.vectra.ai/api-recipes/readme.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netography/refs/heads/main/authentication/netography-authentication.yml
summary_line: http-bearer-jwt/api-key-derived · 3 schemes
tags:
- Network Security
- Network Detection and Response
- Cloud Security
- Network Observability
- Flow Data
- Threat Intelligence
- DDoS
- Cybersecurity
- MITRE ATT&CK
- Company
---
