---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Daylight Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Daylight secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Daylight
provider_slug: daylight
scheme_count: 2
schemes:
- applies_to: https://api.daylight.ai
  authorization_endpoint: https://auth.app.daylight.ai/oauth2/v1/apps/authorize
  bearer_methods_supported:
  - header
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
  code_challenge_methods_supported:
  - S256
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
  - urn:openid:params:grant-type:ciba
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://auth.app.daylight.ai/v1/apps/Peuc12rtvwjSr4gXbIvmOHyv8UyFi29b
  jwks_uri: https://auth.app.daylight.ai/Peuc12rtvwjSr4gXbIvmOHyv8UyFi29b/.well-known/jwks.json
  name: daylight-api-oidc
  registration_endpoint: https://auth.app.daylight.ai/v1/mgmt/inboundapp/app/Peuc12rtvwjSr4gXbIvmOHyv8UyFi29b/register
  response_types_supported:
  - code
  revocation_endpoint: https://auth.app.daylight.ai/oauth2/v1/apps/revoke
  scopes_supported:
  - openid
  token_endpoint: https://auth.app.daylight.ai/oauth2/v1/apps/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://auth.app.daylight.ai/oauth2/v1/apps/userinfo
- applies_to: https://docs.daylight.ai/mcp
  authorization_endpoint: https://docs.daylight.ai/mcp/oauth/authorize
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  issuer: https://docs.daylight.ai/mcp/oauth
  name: daylight-docs-mcp-oauth
  registration_endpoint: https://docs.daylight.ai/mcp/oauth/register
  response_types_supported:
  - code
  scopes_supported:
  - mcp:search
  token_endpoint: https://docs.daylight.ai/mcp/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: daylight-authentication
source_filename: daylight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://api.daylight.ai/.well-known/oauth-protected-resource +\n  https://auth.app.daylight.ai/v1/apps/Peuc12rtvwjSr4gXbIvmOHyv8UyFi29b/.well-known/openid-configuration +\n  https://docs.daylight.ai/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2, openIdConnect]\n  bearer_methods: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  notes: >-\n    No public API keys or docs auth page; the product API is OAuth2/OIDC only.\n    Discovery metadata indicates a Stytch \"Connected Apps\" authorization server.\nschemes:\n- name: daylight-api-oidc\n  type: openIdConnect\n  applies_to: https://api.daylight.ai\n  bearer_methods_supported: [header]\n  scopes_supported: [openid]\n  issuer: https://auth.app.daylight.ai/v1/apps/Peuc12rtvwjSr4gXbIvmOHyv8UyFi29b\n  authorization_endpoint: https://auth.app.daylight.ai/oauth2/v1/apps/authorize\n  token_endpoint: https://auth.app.daylight.ai/oauth2/v1/apps/token\n\
  \  userinfo_endpoint: https://auth.app.daylight.ai/oauth2/v1/apps/userinfo\n  revocation_endpoint: https://auth.app.daylight.ai/oauth2/v1/apps/revoke\n  jwks_uri: https://auth.app.daylight.ai/Peuc12rtvwjSr4gXbIvmOHyv8UyFi29b/.well-known/jwks.json\n  registration_endpoint: https://auth.app.daylight.ai/v1/mgmt/inboundapp/app/Peuc12rtvwjSr4gXbIvmOHyv8UyFi29b/register\n  response_types_supported: [code]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - urn:openid:params:grant-type:ciba\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  dpop_signing_alg_values_supported: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512, EdDSA]\n  claims_supported: [iss, aud, iat, exp, sub, name, email, email_verified,\
  \ phone_number, phone_number_verified, picture, family_name, given_name]\n- name: daylight-docs-mcp-oauth\n  type: oauth2\n  applies_to: https://docs.daylight.ai/mcp\n  issuer: https://docs.daylight.ai/mcp/oauth\n  authorization_endpoint: https://docs.daylight.ai/mcp/oauth/authorize\n  token_endpoint: https://docs.daylight.ai/mcp/oauth/token\n  registration_endpoint: https://docs.daylight.ai/mcp/oauth/register\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, client_credentials, refresh_token]\n  token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  scopes_supported: [mcp:search]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daylight/refs/heads/main/authentication/daylight-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- MDR
- Threat Detection
- Incident Response
- Agentic AI
- SOC
- MCP
---
