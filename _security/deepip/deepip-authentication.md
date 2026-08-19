---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Deepip Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DeepIP secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DeepIP
provider_slug: deepip
scheme_count: 2
schemes:
- applies_to: https://app.deepip.ai/mcp
  client_registration:
    client_id_metadata_document_supported: true
    dynamic_client_registration: false
  flows:
  - authorizationUrl: https://app.deepip.ai/mcp/authorize
    flow: authorizationCode
    revocationUrl: https://app.deepip.ai/mcp/revoke
    scopes: {}
    scopes_note: The authorization-server metadata advertises no scopes_supported array, so the MCP scope vocabulary is not publicly declared.
    tokenUrl: https://app.deepip.ai/mcp/token
  issuer: https://app.deepip.ai/
  name: mcp-oauth2
  pkce:
    code_challenge_methods_supported:
    - S256
    required: true
  presentation:
    challenge: 'WWW-Authenticate: Bearer resource_metadata="https://app.deepip.ai/.well-known/oauth-protected-resource/mcp"'
    header: Authorization
    scheme: Bearer
    unauthenticated_response: 401 {"code":"MISSING_CREDENTIALS","message":"Bearer authentication token is required","requestId":"...","status":"error","timestamp":"..."}
  source: well-known/deepip-app-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
  type: oauth2
- applies_to: https://app.deepip.ai (end-user application sign-in)
  backchannel_logout_supported: true
  code_challenge_methods_supported:
  - S256
  - plain
  endpoints:
    authorization: https://auth.deepip.ai/authorize
    device_authorization: https://auth.deepip.ai/oauth/device/code
    end_session: https://auth.deepip.ai/oidc/logout
    jwks: https://auth.deepip.ai/.well-known/jwks.json
    mfa_challenge: https://auth.deepip.ai/mfa/challenge
    registration: https://auth.deepip.ai/oidc/register
    revocation: https://auth.deepip.ai/oauth/revoke
    token: https://auth.deepip.ai/oauth/token
    userinfo: https://auth.deepip.ai/userinfo
  grant_types_supported:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.deepip.ai/
  mfa: An mfa_challenge endpoint and MFA grant types (mfa-oob, mfa-otp, mfa-recovery-code) are advertised, so multi-factor is available on the tenant.
  name: deepip-auth0-oidc
  openIdConnectUrl: https://auth.deepip.ai/.well-known/openid-configuration
  provider: Auth0 tenant on auth.deepip.ai
  source: well-known/deepip-auth-openid-configuration.json
  type: openIdConnect
slug: deepip-authentication
source_filename: deepip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: >-\n  https://app.deepip.ai/.well-known/oauth-authorization-server,\n  https://app.deepip.ai/.well-known/oauth-protected-resource/mcp,\n  https://auth.deepip.ai/.well-known/openid-configuration\nnote: >-\n  DERIVED FROM DISCOVERY METADATA, NOT FROM AN OPENAPI. DeepIP publishes no\n  machine-readable REST contract, so there are no OpenAPI securitySchemes to\n  aggregate. Both profiles below were read verbatim from discovery documents the\n  provider serves anonymously.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce_required: true\n  bearer_token: true\nschemes:\n- name: mcp-oauth2\n  type: oauth2\n  applies_to: https://app.deepip.ai/mcp\n  source: well-known/deepip-app-oauth-authorization-server.json\n  issuer: https://app.deepip.ai/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.deepip.ai/mcp/authorize\n    tokenUrl: https://app.deepip.ai/mcp/token\n\
  \    revocationUrl: https://app.deepip.ai/mcp/revoke\n    scopes: {}\n    scopes_note: >-\n      The authorization-server metadata advertises no scopes_supported array, so\n      the MCP scope vocabulary is not publicly declared.\n  pkce:\n    required: true\n    code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_post, none]\n  client_registration:\n    dynamic_client_registration: false\n    client_id_metadata_document_supported: true\n  presentation:\n    header: Authorization\n    scheme: Bearer\n    challenge: >-\n      WWW-Authenticate: Bearer resource_metadata=\"https://app.deepip.ai/.well-known/oauth-protected-resource/mcp\"\n    unauthenticated_response: >-\n      401 {\"code\":\"MISSING_CREDENTIALS\",\"message\":\"Bearer authentication token is\n      required\",\"requestId\":\"...\",\"status\":\"error\",\"timestamp\":\"...\"}\n- name: deepip-auth0-oidc\n  type: openIdConnect\n  applies_to: https://app.deepip.ai (end-user application\
  \ sign-in)\n  openIdConnectUrl: https://auth.deepip.ai/.well-known/openid-configuration\n  source: well-known/deepip-auth-openid-configuration.json\n  provider: Auth0 tenant on auth.deepip.ai\n  issuer: https://auth.deepip.ai/\n  endpoints:\n    authorization: https://auth.deepip.ai/authorize\n    token: https://auth.deepip.ai/oauth/token\n    userinfo: https://auth.deepip.ai/userinfo\n    jwks: https://auth.deepip.ai/.well-known/jwks.json\n    registration: https://auth.deepip.ai/oidc/register\n    revocation: https://auth.deepip.ai/oauth/revoke\n    end_session: https://auth.deepip.ai/oidc/logout\n    device_authorization: https://auth.deepip.ai/oauth/device/code\n    mfa_challenge: https://auth.deepip.ai/mfa/challenge\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  code_challenge_methods_supported: [S256, plain]\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  backchannel_logout_supported: true\n  mfa: >-\n    An mfa_challenge endpoint and MFA grant types (mfa-oob, mfa-otp,\n    mfa-recovery-code) are advertised, so multi-factor is available on the tenant.\ngaps:\n- >-\n  No API-key mechanism is documented publicly. DeepIP's security page advertises\n  \"a comprehensive, well-documented API\" for custom integrations, but the\n  reference lives at docs.deepip.ai behind a ReadMe login (redirects to\n  dash.readme.com/to/getdavinci), so its credential model could not be read.\n- >-\n  The MCP authorization server declares no scopes_supported, so the permission\n  granularity an agent is consenting to is not knowable before the consent\n  screen.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepip/refs/heads/main/authentication/deepip-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Intellectual Property
- Patents
- Legal Tech
- Artificial Intelligence
- Patent Drafting
- IP Management
- Document Automation
- Security
- MCP
- Agents
- Prior Art Search
---
