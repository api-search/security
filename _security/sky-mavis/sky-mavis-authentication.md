---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Sky Mavis Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- implicit
overview: Sky Mavis secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, and implicit flow(s).
provider_name: Sky Mavis
provider_slug: sky-mavis
scheme_count: 3
schemes:
- applies_to:
  - Ronin Skynet Web3 API
  - Axie Infinity Origins API
  - AXP API
  - Ronin Market Partner API
  - Ronin Store API
  description: API-gateway products (Skynet Web3 API, Origins/AXP, Ronin Market/Store partner APIs, gateway JSON-RPC) require an X-API-KEY header. Keys are issued per app from the Ronin Developer Console. A request without a key returns HTTP 401 with body {"message":"No API key found in request"}.
  in: header
  name: SkynetApiKey
  parameter_name: X-API-KEY
  type: apiKey
- authorization_endpoint: https://athena.skymavis.com/oauth2/auth
  description: Ronin Waypoint is an OAuth2 / OpenID Connect account service and keyless wallet used to onboard players into Ronin games. PKCE is supported (code_challenge_methods_supported present in discovery).
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  issuer: https://athena.skymavis.com/
  jwks_uri: https://athena.skymavis.com/.well-known/jwks.json
  name: RoninWaypointOIDC
  openid_connect_url: https://athena.skymavis.com/.well-known/openid-configuration
  pkce: true
  token_endpoint: https://athena.skymavis.com/oauth2/token
  type: openIdConnect
- description: 'The public Ronin mainnet JSON-RPC endpoint (https://api.roninchain.com/rpc) is reachable without a key for read/broadcast calls (verified: eth_chainId returns 0x7e4 / chain 2020). Higher rate limits and archive access are served through the authenticated api-gateway.skymavis.com JSON-RPC surface.'
  name: PublicJSONRPC
  type: none
slug: sky-mavis-authentication
source_filename: sky-mavis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.skymavis.com/ + https://athena.skymavis.com/.well-known/openid-configuration + live 401 probe\ndocs: https://docs.skymavis.com/get-started#get-api-key\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, implicit]\nschemes:\n- name: SkynetApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  description: >-\n    API-gateway products (Skynet Web3 API, Origins/AXP, Ronin Market/Store partner\n    APIs, gateway JSON-RPC) require an X-API-KEY header. Keys are issued per app\n    from the Ronin Developer Console. A request without a key returns HTTP 401 with\n    body {\"message\":\"No API key found in request\"}.\n  applies_to:\n  - Ronin Skynet Web3 API\n  - Axie Infinity Origins API\n  - AXP API\n  - Ronin Market Partner API\n  - Ronin Store API\n- name: RoninWaypointOIDC\n  type: openIdConnect\n  openid_connect_url:\
  \ https://athena.skymavis.com/.well-known/openid-configuration\n  issuer: https://athena.skymavis.com/\n  authorization_endpoint: https://athena.skymavis.com/oauth2/auth\n  token_endpoint: https://athena.skymavis.com/oauth2/token\n  jwks_uri: https://athena.skymavis.com/.well-known/jwks.json\n  grant_types: [authorization_code, client_credentials, refresh_token, implicit]\n  pkce: true\n  description: >-\n    Ronin Waypoint is an OAuth2 / OpenID Connect account service and keyless\n    wallet used to onboard players into Ronin games. PKCE is supported\n    (code_challenge_methods_supported present in discovery).\n- name: PublicJSONRPC\n  type: none\n  description: >-\n    The public Ronin mainnet JSON-RPC endpoint (https://api.roninchain.com/rpc)\n    is reachable without a key for read/broadcast calls (verified: eth_chainId\n    returns 0x7e4 / chain 2020). Higher rate limits and archive access are served\n    through the authenticated api-gateway.skymavis.com JSON-RPC surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sky-mavis/refs/heads/main/authentication/sky-mavis-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Blockchain
- Web3
- Gaming
- NFT
- Wallet
- JSON-RPC
- Cryptocurrency
- Developer Tools
---
