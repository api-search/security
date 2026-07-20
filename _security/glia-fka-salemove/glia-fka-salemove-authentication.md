---
api_key_in: []
auth_types:
- bearer
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Glia Fka Salemove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glia (fka SaleMove) secures its APIs with bearer and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Glia (fka SaleMove)
provider_slug: glia-fka-salemove
scheme_count: 2
schemes:
- description: Requests to the Glia REST API authenticate with a bearer token in the Authorization header. A 401 triggers an automatic token refresh in the first-party client.
  format: Bearer <token>
  header: Authorization
  in: header
  name: bearerToken
  scheme: bearer
  type: http
- description: A Glia API Key (key id + secret) plus a Site ID is exchanged for a short-lived bearer token via POST https://api.glia.com/operator_authentication/tokens. Token validity is checked at GET https://api.glia.com/operator_authentication/sessions/current.
  name: apiKeyExchange
  required_credentials:
  - site_id
  - api_key_id
  - api_key_secret
  session_endpoint: https://api.glia.com/operator_authentication/sessions/current
  token_endpoint: https://api.glia.com/operator_authentication/tokens
  type: apiKey
slug: glia-fka-salemove-authentication
source_filename: glia-fka-salemove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  Glia Functions CLI API client (github.com/salemove/glia-functions-tools,\n  src/lib/config.js + src/lib/api.js). No public OpenAPI was reachable; the auth\n  model is captured from the first-party API client source.\ndocs: https://docs.glia.com\napi_base: https://api.glia.com\nsummary:\n  types: [bearer, apiKey]\n  token_style: bearer-token-exchange\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <token>'\n  description: >-\n    Requests to the Glia REST API authenticate with a bearer token in the\n    Authorization header. A 401 triggers an automatic token refresh in the\n    first-party client.\n- name: apiKeyExchange\n  type: apiKey\n  description: >-\n    A Glia API Key (key id + secret) plus a Site ID is exchanged for a\n    short-lived bearer token via POST https://api.glia.com/operator_authentication/tokens.\n    Token validity is checked\
  \ at GET https://api.glia.com/operator_authentication/sessions/current.\n  token_endpoint: https://api.glia.com/operator_authentication/tokens\n  session_endpoint: https://api.glia.com/operator_authentication/sessions/current\n  required_credentials: [site_id, api_key_id, api_key_secret]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glia-fka-salemove/refs/heads/main/authentication/glia-fka-salemove-authentication.yml
summary_line: bearer/apiKey · 2 schemes
tags:
- Company
- Customer Service
- Customer Support
- Digital Customer Service
- Contact Center
- Conversational AI
- Voice AI
- Co-Browsing
- Financial Services
- Banking
- Serverless
- SDK
---
