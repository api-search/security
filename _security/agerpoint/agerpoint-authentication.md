---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Agerpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agerpoint declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Agerpoint
provider_slug: agerpoint
scheme_count: 2
schemes:
- description: OAuth 2.0 bearer access token (RS256 JWT) minted by the Agerpoint Auth0 tenant. The API is registered in Auth0 as the resource identified by the audience https://cloudapi.agerpoint.com.
  evidence: 'HTTP 401 + WWW-Authenticate: Bearer on GET https://cloudapi.agerpoint.com/api/Capture/{id}'
  format: Bearer <JWT>
  header: Authorization
  in: header
  name: oauth2_auth0
  type: oauth2
- description: Full OIDC discovery is served anonymously by the tenant, including JWKS, userinfo, device authorization, back-channel authentication and global token revocation endpoints.
  name: openIdConnect
  openIdConnectUrl: https://agerpoint.us.auth0.com/.well-known/openid-configuration
  type: openIdConnect
slug: agerpoint-authentication
source_filename: agerpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://agerpoint.us.auth0.com/.well-known/openid-configuration (HTTP 200, saved verbatim to\n  well-known/agerpoint-openid-configuration.json) plus an unauthenticated probe of\n  https://cloudapi.agerpoint.com/api/Capture/{id} which answered HTTP 401 with \"WWW-Authenticate: Bearer\",\n  and the Auth0 client configuration published in the first-party console bundle\n  https://cloud.agerpoint.com/assets/index-BtaS8OkR.js\napi: Agerpoint Cloud API\nsummary: >-\n  Every Agerpoint Cloud API operation is protected by an OAuth 2.0 / OpenID Connect bearer token issued by\n  the Auth0 tenant agerpoint.us.auth0.com for the audience https://cloudapi.agerpoint.com. Agerpoint\n  publishes no developer-facing authentication guide, no API-key mechanism, and no public client\n  registration; credentials are provisioned to tenants, so this profile is read from the authorization\n  server's own discovery document rather than from documentation.\n\
  published_documentation: false\ndocumentation_note: >-\n  No public auth reference exists. www.agerpoint.com/developers, /docs and /api all return HTTP 404;\n  cloud.agerpoint.com is a login-gated single-page console.\nschemes:\n- name: oauth2_auth0\n  type: oauth2\n  in: header\n  header: Authorization\n  format: Bearer <JWT>\n  description: >-\n    OAuth 2.0 bearer access token (RS256 JWT) minted by the Agerpoint Auth0 tenant. The API is registered\n    in Auth0 as the resource identified by the audience https://cloudapi.agerpoint.com.\n  evidence: 'HTTP 401 + WWW-Authenticate: Bearer on GET https://cloudapi.agerpoint.com/api/Capture/{id}'\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://agerpoint.us.auth0.com/.well-known/openid-configuration\n  description: >-\n    Full OIDC discovery is served anonymously by the tenant, including JWKS, userinfo, device\n    authorization, back-channel authentication and global token revocation endpoints.\nauthorization_server:\n\
  \  issuer: https://agerpoint.us.auth0.com/\n  vendor: Auth0 (Okta)\n  region: us\n  discovery: https://agerpoint.us.auth0.com/.well-known/openid-configuration\n  rfc8414_alias: https://agerpoint.us.auth0.com/.well-known/oauth-authorization-server\n  rfc8414_identical_to_oidc: true\n  endpoints:\n    authorization: https://agerpoint.us.auth0.com/authorize\n    token: https://agerpoint.us.auth0.com/oauth/token\n    userinfo: https://agerpoint.us.auth0.com/userinfo\n    jwks: https://agerpoint.us.auth0.com/.well-known/jwks.json\n    revocation: https://agerpoint.us.auth0.com/oauth/revoke\n    registration: https://agerpoint.us.auth0.com/oidc/register\n    device_authorization: https://agerpoint.us.auth0.com/oauth/device/code\n    backchannel_authentication: https://agerpoint.us.auth0.com/bc-authorize\n    end_session: https://agerpoint.us.auth0.com/oidc/logout\n    mfa_challenge: https://agerpoint.us.auth0.com/mfa/challenge\n    global_token_revocation: https://agerpoint.us.auth0.com/oauth/global-token-revocation/connection/{connectionName}\n\
  \  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types_supported:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n  dpop:\n    supported: true\n    signing_algs:\n    - ES256\n  id_token_signing_alg_values_supported:\n  - HS256\n\
  \  - RS256\n  - PS256\n  mfa: true\n  dynamic_client_registration: true\nclients_observed:\n- name: Agerpoint Cloud console\n  type: public SPA (authorization code + PKCE)\n  callback: https://cloud.agerpoint.com\n  audience: https://cloudapi.agerpoint.com\n  source: https://cloud.agerpoint.com/assets/index-BtaS8OkR.js\ngaps:\n- No public documentation of how a customer or partner obtains client credentials.\n- No API-key alternative is offered or documented.\n- No published scope reference for the https://cloudapi.agerpoint.com resource (see scopes/).\n- No /.well-known/oauth-protected-resource (RFC 9728) on cloudapi.agerpoint.com (HTTP 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agerpoint/refs/heads/main/authentication/agerpoint-authentication.yml
summary_line: 2 schemes
tags:
- Agriculture
- Geospatial
- Remote Sensing
- Digital Twin
- LiDAR
- Point Cloud
- Carbon Measurement
- Forestry
- Machine Learning
- Spatial Analytics
- Company
---
