---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Provable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Provable secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Provable
provider_slug: provable
scheme_count: 2
schemes:
- description: Clients authenticate by calling LoginService/LoginWithApiCredentials with issued API credentials, which returns a bearer access token (TTL ~1 week) used on subsequent Aurora API calls.
  login_operation: LoginService/LoginWithApiCredentials
  name: ApiCredentialsLogin
  sources:
  - https://developer.provablemarkets.com/api/connectapi/loginservice/loginwithapicredentials
  type: apiKey
- description: Access token returned by the login service, presented as a bearer token on Connect API calls.
  name: BearerAccessToken
  scheme: bearer
  sources:
  - https://developer.provablemarkets.com/workflows
  type: http
slug: provable-authentication
source_filename: provable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.provablemarkets.com/api/connectapi/loginservice/loginwithapicredentials\ndocs: https://developer.provablemarkets.com/workflows\nsummary:\n  api_style: grpc-connect            # Connect protocol (gRPC, gRPC-Web, Connect-HTTP)\n  types: [apiKey, http]\n  api_key_in: [header]\n  access_token_ttl: 1 week\nschemes:\n  - name: ApiCredentialsLogin\n    type: apiKey\n    description: >-\n      Clients authenticate by calling LoginService/LoginWithApiCredentials with\n      issued API credentials, which returns a bearer access token (TTL ~1 week)\n      used on subsequent Aurora API calls.\n    login_operation: LoginService/LoginWithApiCredentials\n    sources: [https://developer.provablemarkets.com/api/connectapi/loginservice/loginwithapicredentials]\n  - name: BearerAccessToken\n    type: http\n    scheme: bearer\n    description: Access token returned by the login service, presented as a bearer token on Connect\
  \ API calls.\n    sources: [https://developer.provablemarkets.com/workflows]\nevent_delivery_auth:\n  description: >-\n    Unsolicited event delivery (Webhook, RPCHooks, WebSocket) supports its own\n    authentication so Provable can authenticate to the customer endpoint / the\n    customer can authenticate the stream.\n  webhook: [basic, hmac-sha256, api-key-header]     # X-API-KEY\n  rpchooks: [basic, hmac-sha256, api-key-header]\n  websocket:\n    endpoint: wss://provablemarkets.com/api/1/websocket/events\n    auth: bearer-api-key\n    extra_header: X-CONNECTION-CONFIG-ID\nnotes:\n  - No public OAuth2/OIDC flow is documented for the Aurora API itself; the\n    developer.provablemarkets.com/.well-known/oauth-authorization-server document\n    is the Redocly portal's own MCP OAuth surface, not the trading API's auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provable/refs/heads/main/authentication/provable-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Securities Lending
- Capital Markets
- Fintech
- Trading
- Alternative Trading System
- Post-Trade
- gRPC
- FIX
---
