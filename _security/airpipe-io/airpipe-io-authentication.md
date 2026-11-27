---
anonymous_access: false
api_key_in: []
api_specs:
- filename: airpipe-io-examples-openapi-generated.yml
  format: yaml
  label: Air Pipe Examples API
  slug: examples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airpipe-io/openapi/_ae-authored/airpipe-io-examples-openapi-generated.yml
- filename: airpipe-io-tutorial-openapi-generated.yml
  format: yaml
  label: Air Pipe tutorial API
  slug: tutorial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airpipe-io/openapi/_ae-authored/airpipe-io-tutorial-openapi-generated.yml
auth_types: []
description: Authentication methods documented for Air Pipe
kind: authentication
layout: security
mechanism_count: 9
method: searched
name: Air Pipe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Air Pipe declares 9 security scheme(s) across its OpenAPI definitions.
provider_name: Air Pipe
provider_slug: airpipe-io
scheme_count: 9
schemes:
- evidence: 'Backend (WS): the org API key via Authorization: Bearer , x-api-key , or ?api_key= .'
  header: Authorization
  how_to_obtain: Issued by Air Pipe as an organization API key; used server‑to‑server.
  location: header
  name: Backend API key
  type: http-bearer
- evidence: 'Backend (WS): the org API key via Authorization: Bearer , x-api-key , or ?api_key= .'
  header: x-api-key
  how_to_obtain: Issued by Air Pipe as an organization API key; used server‑to‑server.
  location: header
  name: Backend API key (alternative header)
  type: http-bearer
- evidence: 'Backend (WS): the org API key via Authorization: Bearer , x-api-key , or ?api_key= .'
  how_to_obtain: Issued by Air Pipe as an organization API key; passed as ?api_key=.
  location: query
  name: Backend API key (query)
  type: http-bearer
- evidence: 'WebSocket, native: the airpipe-jwt header (or ?token= ).'
  header: airpipe-jwt
  how_to_obtain: Minted by Air Pipe via add_jwt after user login; signed with a shared secret.
  location: header
  name: JWT (shared secret)
  type: http-bearer
- evidence: 'WebSocket, browser: ?token=<jwt> on the URL — browsers can''t set WebSocket headers.'
  how_to_obtain: Minted by Air Pipe via add_jwt after user login; signed with a shared secret.
  location: query
  name: JWT (shared secret query)
  type: http-bearer
- evidence: Your JWT — JWKS Verified against your IdP's JWKS (RS256/ES256).
  header: airpipe-jwt
  how_to_obtain: Issued by external IdP; verified against JWKS URL configured in Air Pipe.
  location: header
  name: JWT (JWKS)
  type: http-bearer
- authorize_url: https://accounts.google.com/o/oauth2/v2/auth
  evidence: The OAuth2 authorization code flow with refresh, per user.
  header: Authorization
  how_to_obtain: User initiates flow via /oauth/start, consents at provider, callback exchanges code for tokens.
  location: header
  name: OAuth2 Authorization Code
  token_url: https://oauth2.googleapis.com/token
  type: http-bearer
- evidence: 'This basic auth is passed in the Authorization header

    Basic U2luY2VyZUBhcHJpbC5iaXo6bXlwYXNzd29yZA=='
  header: Authorization
  how_to_obtain: Client supplies Base64‑encoded username:password in Authorization header.
  location: header
  name: Basic Auth
  type: http-basic
- evidence: 'MQTT: username = <ORG_UUID> , password = <API_KEY> — or no password for public .'
  how_to_obtain: Username is organization UUID; password is organization API key.
  location: username_password
  name: MQTT credentials
  type: other
slug: airpipe-io-authentication
source_filename: airpipe-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.airpipe.io/docs/features/realtime/realtime-auth/
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.airpipe.io/docs/features/realtime/realtime-auth/\nsources:\n- https://docs.airpipe.io/docs/features/realtime/realtime-auth/\n- https://docs.airpipe.io/docs/examples/marketplace/oauth-connect/\n- https://docs.airpipe.io/docs/tutorial/authorization/jwt/\n- https://docs.airpipe.io/docs/tutorial/authorization/basic-auth/\ndescription: Authentication methods documented for Air Pipe\nschemes:\n- type: http-bearer\n  name: Backend API key\n  evidence: 'Backend (WS): the org API key via Authorization: Bearer , x-api-key , or ?api_key= .'\n  location: header\n  header: Authorization\n  how_to_obtain: Issued by Air Pipe as an organization API key; used server‑to‑server.\n- type: http-bearer\n  name: Backend API key (alternative header)\n  evidence: 'Backend (WS): the org API key via Authorization: Bearer , x-api-key , or ?api_key= .'\n  location: header\n  header: x-api-key\n\
  \  how_to_obtain: Issued by Air Pipe as an organization API key; used server‑to‑server.\n- type: http-bearer\n  name: Backend API key (query)\n  evidence: 'Backend (WS): the org API key via Authorization: Bearer , x-api-key , or ?api_key= .'\n  location: query\n  how_to_obtain: Issued by Air Pipe as an organization API key; passed as ?api_key=.\n- type: http-bearer\n  name: JWT (shared secret)\n  evidence: 'WebSocket, native: the airpipe-jwt header (or ?token= ).'\n  location: header\n  header: airpipe-jwt\n  how_to_obtain: Minted by Air Pipe via add_jwt after user login; signed with a shared secret.\n- type: http-bearer\n  name: JWT (shared secret query)\n  evidence: 'WebSocket, browser: ?token=<jwt> on the URL — browsers can''t set WebSocket headers.'\n  location: query\n  how_to_obtain: Minted by Air Pipe via add_jwt after user login; signed with a shared secret.\n- type: http-bearer\n  name: JWT (JWKS)\n  evidence: Your JWT — JWKS Verified against your IdP's JWKS (RS256/ES256).\n \
  \ location: header\n  header: airpipe-jwt\n  how_to_obtain: Issued by external IdP; verified against JWKS URL configured in Air Pipe.\n- type: http-bearer\n  name: OAuth2 Authorization Code\n  evidence: The OAuth2 authorization code flow with refresh, per user.\n  location: header\n  header: Authorization\n  token_url: https://oauth2.googleapis.com/token\n  authorize_url: https://accounts.google.com/o/oauth2/v2/auth\n  how_to_obtain: User initiates flow via /oauth/start, consents at provider, callback exchanges code for tokens.\n- type: http-basic\n  name: Basic Auth\n  evidence: 'This basic auth is passed in the Authorization header\n\n    Basic U2luY2VyZUBhcHJpbC5iaXo6bXlwYXNzd29yZA=='\n  location: header\n  header: Authorization\n  how_to_obtain: Client supplies Base64‑encoded username:password in Authorization header.\n- type: other\n  name: MQTT credentials\n  evidence: 'MQTT: username = <ORG_UUID> , password = <API_KEY> — or no password for public .'\n  location: username_password\n\
  \  how_to_obtain: Username is organization UUID; password is organization API key.\ndocs: https://docs.airpipe.io/docs/features/realtime/realtime-auth/\n"
source_yaml_url: https://artifacts.apis.io/airpipe-io/authentication/airpipe-io-authentication.yml
summary_line: 9 schemes
tags:
- Platform
- Automation
- Artificial Intelligence
- Backend
- Company
---
