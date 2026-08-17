---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Regieai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Regie.ai declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Regie.ai
provider_slug: regieai
scheme_count: 4
schemes:
- additional_identifiers:
  - user ID
  - workspace ID
  applies_to: https://mcp.regie.ai
  documented_publicly: false
  evidence: Anonymous requests return 401 "Missing required API key". Requests carrying an x-api-key header return 401 "Missing required user ID or workspace ID", proving a two-stage check of key plus workspace/user identity.
  id: mcp-api-key
  in: header
  name: x-api-key
  type: apiKey
- applies_to:
  - https://sales-prod-api.regie.ai
  - https://agents-api.regie.ai
  - https://dialer-api.regie.ai
  - https://transcript-api.regie.ai
  - https://user-management.regie.ai
  - https://marketing-api.regie.ai
  documented_publicly: false
  evidence: Every non-health path on these hosts returns 401 "Authorization header not provided in the request". These are the first-party application backends behind app.regie.ai, not a published developer API.
  id: backend-bearer
  in: header
  name: Authorization
  scheme: bearer
  type: http
- applies_to: end-user sign-in to app.regie.ai (login/callback)
  authorization_endpoint: https://authenticate.regie.ai/authorize
  code_challenge_methods_supported:
  - S256
  - plain
  documented_publicly: false
  evidence: app.regie.ai's application bundle points its login callback at https://authenticate.regie.ai/login/callback; the tenant serves a full OIDC discovery document at HTTP 200.
  grant_types_supported:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: auth0-oidc
  issuer: https://authenticate.regie.ai/
  jwks_uri: https://authenticate.regie.ai/.well-known/jwks.json
  openIdConnectUrl: https://authenticate.regie.ai/.well-known/openid-configuration
  provider: Auth0
  registration_endpoint: https://authenticate.regie.ai/oidc/register
  revocation_endpoint: https://authenticate.regie.ai/oauth/revoke
  scopes_supported:
  - openid
  - profile
  - offline_access
  - name
  - given_name
  - family_name
  - nickname
  - email
  - email_verified
  - picture
  - created_at
  - identities
  - phone
  - address
  token_endpoint: https://authenticate.regie.ai/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://authenticate.regie.ai/userinfo
- applies_to: second identity tenant on the regie.ai domain (WorkOS AuthKit)
  authorization_endpoint: https://authkit.regie.ai/oauth2/authorize
  device_authorization_endpoint: https://authkit.regie.ai/oauth2/device_authorization
  documented_publicly: false
  evidence: OIDC discovery document served at HTTP 200 from the company's own host.
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id: workos-authkit-oidc
  introspection_endpoint: https://authkit.regie.ai/oauth2/introspection
  issuer: https://authkit.regie.ai
  jwks_uri: https://authkit.regie.ai/oauth2/jwks
  openIdConnectUrl: https://authkit.regie.ai/.well-known/openid-configuration
  provider: WorkOS AuthKit
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  token_endpoint: https://authkit.regie.ai/oauth2/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://authkit.regie.ai/oauth2/userinfo
slug: regieai-authentication
source_filename: regieai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://authenticate.regie.ai/.well-known/openid-configuration,\n  https://authkit.regie.ai/.well-known/openid-configuration, and live 401 responses from\n  mcp.regie.ai, sales-prod-api.regie.ai, agents-api.regie.ai (probed 2026-08-14)\nnote: >-\n  Regie.ai publishes no OpenAPI and no public developer authentication documentation, so this\n  profile is assembled entirely from documents and error responses the company's own hosts\n  served to an anonymous client. Nothing here is inferred from marketing copy.\nschemes:\n- id: mcp-api-key\n  type: apiKey\n  in: header\n  name: x-api-key\n  applies_to: https://mcp.regie.ai\n  additional_identifiers:\n  - user ID\n  - workspace ID\n  evidence: >-\n    Anonymous requests return 401 \"Missing required API key\". Requests carrying an x-api-key\n    header return 401 \"Missing required user ID or workspace ID\", proving a two-stage check of\n    key plus workspace/user identity.\n\
  \  documented_publicly: false\n- id: backend-bearer\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  applies_to:\n  - https://sales-prod-api.regie.ai\n  - https://agents-api.regie.ai\n  - https://dialer-api.regie.ai\n  - https://transcript-api.regie.ai\n  - https://user-management.regie.ai\n  - https://marketing-api.regie.ai\n  evidence: >-\n    Every non-health path on these hosts returns 401 \"Authorization header not provided in the\n    request\". These are the first-party application backends behind app.regie.ai, not a\n    published developer API.\n  documented_publicly: false\n- id: auth0-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://authenticate.regie.ai/.well-known/openid-configuration\n  provider: Auth0\n  issuer: https://authenticate.regie.ai/\n  authorization_endpoint: https://authenticate.regie.ai/authorize\n  token_endpoint: https://authenticate.regie.ai/oauth/token\n  userinfo_endpoint: https://authenticate.regie.ai/userinfo\n  jwks_uri:\
  \ https://authenticate.regie.ai/.well-known/jwks.json\n  registration_endpoint: https://authenticate.regie.ai/oidc/register\n  revocation_endpoint: https://authenticate.regie.ai/oauth/revoke\n  scopes_supported:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  applies_to: end-user sign-in to app.regie.ai (login/callback)\n  evidence: >-\n    app.regie.ai's application bundle points its login\
  \ callback at\n    https://authenticate.regie.ai/login/callback; the tenant serves a full OIDC discovery\n    document at HTTP 200.\n  documented_publicly: false\n- id: workos-authkit-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://authkit.regie.ai/.well-known/openid-configuration\n  provider: WorkOS AuthKit\n  issuer: https://authkit.regie.ai\n  authorization_endpoint: https://authkit.regie.ai/oauth2/authorize\n  token_endpoint: https://authkit.regie.ai/oauth2/token\n  userinfo_endpoint: https://authkit.regie.ai/oauth2/userinfo\n  introspection_endpoint: https://authkit.regie.ai/oauth2/introspection\n  jwks_uri: https://authkit.regie.ai/oauth2/jwks\n  device_authorization_endpoint: https://authkit.regie.ai/oauth2/device_authorization\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  - offline_access\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types_supported:\n\
  \  - code\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  applies_to: second identity tenant on the regie.ai domain (WorkOS AuthKit)\n  evidence: OIDC discovery document served at HTTP 200 from the company's own host.\n  documented_publicly: false\nsummary:\n  public_developer_auth_documented: false\n  api_key_surface: true\n  oauth2_or_oidc_present: true\n  mtls: false\n  sso_providers:\n  - Auth0\n  - WorkOS AuthKit\n  docs: null\n  docs_note: >-\n    There is no public authentication page to link. help.regie.ai is the only documentation\n    surface and it now returns 403 behind a Cloudflare challenge, redirecting to /hc/restricted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regieai/refs/heads/main/authentication/regieai-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Ai Apps
- Sales Engagement
- Sales AI
- Outbound
- Prospecting
- Revenue Operations
- AI Agents
---
