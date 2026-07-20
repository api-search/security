---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Linktree Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
- ciba
- jwtBearer
- tokenExchange
overview: Linktree secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, deviceCode, ciba, jwtBearer, and tokenExchange flow(s).
provider_name: Linktree
provider_slug: linktree
scheme_count: 1
schemes:
- authorization_endpoint: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/authorize
  claims_supported:
  - iss
  - aud
  - iat
  - exp
  - sub
  - name
  - email
  - email_verified
  - phone_number
  - phone_number_verified
  - picture
  - family_name
  - given_name
  dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  - EdDSA
  grant_types_supported:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://mcp.linktr.ee
  jwks_uri: https://ciam.linktr.ee/P32ACVpudk8MNftmpf1LR1pW5k8s/.well-known/jwks.json
  name: LinktreeMCPOAuth2
  registration_endpoint: https://ciam.linktr.ee/v1/mgmt/mcp/client/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/register
  revocation_endpoint: https://ciam.linktr.ee/oauth2/v1/apps/P32ACVpudk8MNftmpf1LR1pW5k8s/revoke
  sources:
  - well-known/linktree-oauth-authorization-server.json
  token_endpoint: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://ciam.linktr.ee/oauth2/v1/apps/P32ACVpudk8MNftmpf1LR1pW5k8s/userinfo
slug: linktree-authentication
source_filename: linktree-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# Authentication profile derived from Linktree's published OAuth metadata.\ngenerated: '2026-07-19'\nmethod: searched\nsource: https://linktr.ee/.well-known/oauth-authorization-server\ndocs: https://mcp.linktr.ee/docs\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, deviceCode, ciba, jwtBearer, tokenExchange]\n  identity_provider: Descope\n  scope_count: 30\n  dynamic_client_registration: true\n  pkce_required_methods: [S256]\n  dpop_supported: true\nschemes:\n  - name: LinktreeMCPOAuth2\n    type: oauth2\n    issuer: https://mcp.linktr.ee\n    authorization_endpoint: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/authorize\n    token_endpoint: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/token\n    userinfo_endpoint: https://ciam.linktr.ee/oauth2/v1/apps/P32ACVpudk8MNftmpf1LR1pW5k8s/userinfo\n    revocation_endpoint:\
  \ https://ciam.linktr.ee/oauth2/v1/apps/P32ACVpudk8MNftmpf1LR1pW5k8s/revoke\n    registration_endpoint: https://ciam.linktr.ee/v1/mgmt/mcp/client/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/register\n    jwks_uri: https://ciam.linktr.ee/P32ACVpudk8MNftmpf1LR1pW5k8s/.well-known/jwks.json\n    grant_types_supported:\n      - \"authorization_code\"\n      - \"refresh_token\"\n      - \"client_credentials\"\n      - \"urn:ietf:params:oauth:grant-type:device_code\"\n      - \"urn:openid:params:grant-type:ciba\"\n      - \"urn:ietf:params:oauth:grant-type:jwt-bearer\"\n      - \"urn:ietf:params:oauth:grant-type:token-exchange\"\n    token_endpoint_auth_methods_supported:\n      - none\n      - client_secret_basic\n      - client_secret_post\n    id_token_signing_alg_values_supported: [RS256]\n    dpop_signing_alg_values_supported: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512, EdDSA]\n    claims_supported: [iss, aud, iat, exp, sub, name, email, email_verified,\
  \ phone_number, phone_number_verified, picture, family_name, given_name]\n    sources: [well-known/linktree-oauth-authorization-server.json]\nprotected_resource:\n  resource: https://mcp.linktr.ee/mcp\n  metadata: https://mcp.linktr.ee/.well-known/oauth-protected-resource\n  bearer_methods_supported: [header]\n  rfc: RFC 9728 (OAuth 2.0 Protected Resource Metadata)\nnotes:\n  - Linktree publishes no public REST API; OAuth here protects the MCP server, not a REST surface.\n  - An unauthenticated call to the MCP endpoint returns 401 with a WWW-Authenticate Bearer challenge carrying resource_metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linktree/refs/heads/main/authentication/linktree-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Media
- Link in Bio
- Creator Economy
- Social Media
- Marketing
- Analytics
- MCP
- Agents
---
