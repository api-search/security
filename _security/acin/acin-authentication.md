---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Acin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acin declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Acin
provider_slug: acin
scheme_count: 4
schemes:
- description: The flow the app.acin.com single-page application uses. PKCE is advertised in code_challenge_methods_supported.
  evidence: https://app-auth.acin.com/.well-known/openid-configuration
  flow: authorizationCode
  id: oauth2_authorization_code_pkce
  pkce: true
  pkce_methods:
  - S256
  - plain
  type: oauth2
- description: Machine-to-machine grant advertised in grant_types_supported; this is the grant a server-to-server integration with the Acin gateway would use. No public documentation states which audiences or scopes are issuable.
  evidence: https://app-auth.acin.com/.well-known/openid-configuration
  flow: clientCredentials
  id: oauth2_client_credentials
  type: oauth2
- description: Full OIDC discovery is published, including userinfo and the signing JWKS.
  evidence: https://app-auth.acin.com/.well-known/openid-configuration
  id: oidc
  openIdConnectUrl: https://app-auth.acin.com/.well-known/openid-configuration
  type: openIdConnect
- bearer_format: JWT
  description: The Azure API Management gateway at apim-prod.acin.com requires an Authorization bearer token. An anonymous request returns HTTP 401 with body {"statusCode":401,"message":"Authorization token is missing or invalid"}.
  evidence: https://apim-prod.acin.com/v1/gateway-graphql
  id: bearer_token
  scheme: bearer
  type: http
slug: acin-authentication
source_filename: acin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  https://app-auth.acin.com/.well-known/openid-configuration and\n  https://app-auth.acin.com/.well-known/oauth-authorization-server (both HTTP 200, fetched\n  anonymously 2026-09-06), plus the HTTP 401 challenge returned by\n  https://apim-prod.acin.com/v1/gateway-graphql. Acin publishes no OpenAPI, so no securityScheme\n  block could be derived; every statement below is read off a document the provider serves or a\n  live response observed from its gateway.\nnote: >-\n  Acin does not run a public developer program, so there is no API-key onboarding, no documented\n  auth guide, and no reference. Access to the platform API is OAuth 2.0 / OIDC through Acin's own\n  Auth0 custom domain, and tokens are issued only to an authenticated tenant user or a registered\n  client. Nothing here was inferred from marketing prose.\nauthorization_server:\n  issuer: https://app-auth.acin.com/\n  host: app-auth.acin.com\n  vendor: Auth0 (custom\
  \ domain on the provider's own registrable domain)\n  discovery:\n  - url: https://app-auth.acin.com/.well-known/openid-configuration\n    status: 200\n    file: well-known/acin-openid-configuration.json\n  - url: https://app-auth.acin.com/.well-known/oauth-authorization-server\n    status: 200\n    file: well-known/acin-oauth-authorization-server.json\n  endpoints:\n    authorization: https://app-auth.acin.com/authorize\n    token: https://app-auth.acin.com/oauth/token\n    userinfo: https://app-auth.acin.com/userinfo\n    jwks: https://app-auth.acin.com/.well-known/jwks.json\n    revocation: https://app-auth.acin.com/oauth/revoke\n    registration: https://app-auth.acin.com/oidc/register\n    device_authorization: https://app-auth.acin.com/oauth/device/code\n    backchannel_authentication: https://app-auth.acin.com/bc-authorize\n    mfa_challenge: https://app-auth.acin.com/mfa/challenge\nschemes:\n- id: oauth2_authorization_code_pkce\n  type: oauth2\n  flow: authorizationCode\n  pkce:\
  \ true\n  pkce_methods:\n  - S256\n  - plain\n  description: >-\n    The flow the app.acin.com single-page application uses. PKCE is advertised in\n    code_challenge_methods_supported.\n  evidence: https://app-auth.acin.com/.well-known/openid-configuration\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Machine-to-machine grant advertised in grant_types_supported; this is the grant a\n    server-to-server integration with the Acin gateway would use. No public documentation states\n    which audiences or scopes are issuable.\n  evidence: https://app-auth.acin.com/.well-known/openid-configuration\n- id: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://app-auth.acin.com/.well-known/openid-configuration\n  description: Full OIDC discovery is published, including userinfo and the signing JWKS.\n  evidence: https://app-auth.acin.com/.well-known/openid-configuration\n- id: bearer_token\n  type: http\n  scheme: bearer\n  bearer_format:\
  \ JWT\n  description: >-\n    The Azure API Management gateway at apim-prod.acin.com requires an Authorization bearer token.\n    An anonymous request returns HTTP 401 with body\n    {\"statusCode\":401,\"message\":\"Authorization token is missing or invalid\"}.\n  evidence: https://apim-prod.acin.com/v1/gateway-graphql\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\nid_token_signing_alg_values_supported:\n- HS256\n- RS256\n- PS256\ndpop_signing_alg_values_supported:\n- ES256\nmfa: >-\n  An mfa_challenge_endpoint is published and Auth0 MFA grant types\n  (mfa-oob, mfa-otp, mfa-recovery-code) are advertised, so multi-factor authentication is\n  available on the tenant.\ngaps:\n\
  - No public authentication documentation page exists on acin.com or in the published\n  documentation site.\n- No API-key scheme is published; there is no self-service key issuance.\n- The resource server publishes no /.well-known/oauth-protected-resource (probed 404), so an agent\n  cannot discover the authorization server from the API host alone.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acin/refs/heads/main/authentication/acin-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Operational Risk
- Risk Management
- Non-Financial Risk
- Financial Services
- Banking
- Compliance
- Regulatory Technology
- Benchmarking
- Data Standards
---
