---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Corporate Travel Management Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corporate Travel Management secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Corporate Travel Management
provider_slug: corporate-travel-management
scheme_count: 1
schemes:
- backchannel_logout_supported: true
  client_type: 'Public SPA client (`token_endpoint_auth_method: none` is supported and the client id is embedded in the portal page), consistent with authorization code + PKCE from the browser.'
  code_challenge_methods_supported:
  - S256
  - plain
  connection: The portal requests the `SMART-Database-Connection` Auth0 connection (a username/password database connection), so the default CTM Portal login is local credentials rather than a federated enterprise IdP. CTM's technology pages separately assert single sign-on integration with customer systems; no such connection is publicly enumerable.
  dpop_signing_alg_values_supported:
  - ES256
  endpoints:
    authorization: https://travelctm-au-production.au.auth0.com/authorize
    backchannel_authentication: https://travelctm-au-production.au.auth0.com/bc-authorize
    device_authorization: https://travelctm-au-production.au.auth0.com/oauth/device/code
    dynamic_client_registration: https://travelctm-au-production.au.auth0.com/oidc/register
    mfa_challenge: https://travelctm-au-production.au.auth0.com/mfa/challenge
    revocation: https://travelctm-au-production.au.auth0.com/oauth/revoke
    token: https://travelctm-au-production.au.auth0.com/oauth/token
    userinfo: https://travelctm-au-production.au.auth0.com/userinfo
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://travelctm-au-production.au.auth0.com/
  jwks_uri: https://travelctm-au-production.au.auth0.com/.well-known/jwks.json
  mfa: Supported by the tenant — MFA challenge endpoint and mfa-oob / mfa-otp / mfa-recovery-code grant types are advertised. Whether MFA is enforced for CTM Portal users is not publicly observable.
  name: Auth0 OIDC (CTM Portal)
  openIdConnectUrl: https://travelctm-au-production.au.auth0.com/.well-known/openid-configuration
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: corporate-travel-management-authentication
source_filename: corporate-travel-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource:\n- https://travelctm-au-production.au.auth0.com/.well-known/openid-configuration\n- https://travelctm-au-production.au.auth0.com/.well-known/oauth-authorization-server\n- https://www.ctmsmart.com.au/\n- https://portal-host.api.ctmsmart.com/health\nsummary:\n  types: [oauth2, openIdConnect]\n  provider: Auth0 (AU region, production tenant)\n  documented_by_provider: false\n  derived_from_openapi: false\n  note: >-\n    CTM publishes no authentication documentation, because it publishes no API documentation. This\n    profile is probed, not documented: the CTM Portal bootstrap script names the Auth0 tenant, and\n    that tenant serves a complete anonymous OIDC/RFC 8414 discovery document. Everything below comes\n    from those two live sources. No API key, HTTP basic, mTLS or other scheme is published anywhere\n    on a CTM property.\nschemes:\n- name: Auth0 OIDC (CTM Portal)\n  type: openIdConnect\n  issuer: https://travelctm-au-production.au.auth0.com/\n\
  \  openIdConnectUrl: https://travelctm-au-production.au.auth0.com/.well-known/openid-configuration\n  jwks_uri: https://travelctm-au-production.au.auth0.com/.well-known/jwks.json\n  endpoints:\n    authorization: https://travelctm-au-production.au.auth0.com/authorize\n    token: https://travelctm-au-production.au.auth0.com/oauth/token\n    userinfo: https://travelctm-au-production.au.auth0.com/userinfo\n    revocation: https://travelctm-au-production.au.auth0.com/oauth/revoke\n    device_authorization: https://travelctm-au-production.au.auth0.com/oauth/device/code\n    backchannel_authentication: https://travelctm-au-production.au.auth0.com/bc-authorize\n    dynamic_client_registration: https://travelctm-au-production.au.auth0.com/oidc/register\n    mfa_challenge: https://travelctm-au-production.au.auth0.com/mfa/challenge\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n\
  \  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types_supported: [code, token, id_token, code token, code id_token, token id_token, code token id_token]\n  response_modes_supported: [query, fragment, form_post]\n  code_challenge_methods_supported: [S256, plain]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  dpop_signing_alg_values_supported: [ES256]\n  mfa: >-\n    Supported by the tenant — MFA challenge endpoint and mfa-oob / mfa-otp / mfa-recovery-code grant\n    types are advertised. Whether MFA is enforced for CTM Portal users is not publicly\
  \ observable.\n  backchannel_logout_supported: true\n  connection: >-\n    The portal requests the `SMART-Database-Connection` Auth0 connection (a username/password\n    database connection), so the default CTM Portal login is local credentials rather than a\n    federated enterprise IdP. CTM's technology pages separately assert single sign-on integration\n    with customer systems; no such connection is publicly enumerable.\n  client_type: >-\n    Public SPA client (`token_endpoint_auth_method: none` is supported and the client id is embedded\n    in the portal page), consistent with authorization code + PKCE from the browser.\nprotected_resources:\n- name: CTM Portal host API\n  base_url: https://portal-host.api.ctmsmart.com/api\n  scheme: Bearer JWT issued by the Auth0 tenant above (inferred from the SPA's configuration —\n    the API publishes no WWW-Authenticate challenge on unauthenticated public paths).\n  observed:\n  - path: /\n    status: 200\n    body: 'Healthy'\n  - path: /health\n\
  \    status: 500\n    content_type: application/problem+json\n    detail: \"The AuthorizationPolicy named: 'admin' was not found.\"\n    note: >-\n      Confirms an ASP.NET Core application with named authorization policies; the misconfigured\n      policy leaks that authorization is policy-based. No operation is anonymously reachable.\n  - path: /.well-known/oauth-protected-resource\n    status: 404\n  - path: /swagger/v1/swagger.json\n    status: 404\nsignup:\n  self_service: false\n  note: >-\n    There is no developer sign-up, key request, or client registration path for third parties. Auth0\n    dynamic client registration is advertised at the tenant level but is a stock Auth0 endpoint, not\n    a CTM onboarding offer. Portal accounts are provisioned to contracted customers by CTM.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corporate-travel-management/refs/heads/main/authentication/corporate-travel-management-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Travel
- Australia
- Corporate Travel
- Travel Management Company
- Aviation
- NDC
- Distribution
- Booking
- Hotels
- Meetings and Events
---
