---
api_key_in: []
auth_types: []
description: Pixis publishes no public developer API and issues no public API keys. What it does publish, machine-readably, is an OpenID Connect / OAuth 2.0 discovery document at auth.pixis.ai — the Auth0 custom domain behind application login for Prism and the Pixis platform. The profile below is read verbatim from that document plus the Auth0Provider configuration Pixis ships in its own public Prism JavaScript bundle, and confirmed against the 401 an anonymous caller gets from the Pixis application backend.
kind: authentication
layout: security
method: probed
name: Pixis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixis declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pixis
provider_slug: pixis
scheme_count: 2
schemes:
- description: Authorization Code with PKCE is the flow the Pixis Prism SPA uses; the discovery document also advertises client_credentials, device_code, token-exchange and jwt-bearer.
  dpop_signing_alg_values_supported:
  - ES256
  dynamic_client_registration:
    endpoint: https://auth.pixis.ai/oidc/register
    note: Advertised by the discovery document. Auth0 gates this behind a per-tenant toggle; not probed with a write request.
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
  id: oauth2_oidc
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  mfa:
    evidence: mfa_challenge_endpoint plus four mfa-* grant types in the discovery document.
    supported: true
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  protocol: OpenID Connect 1.0 / OAuth 2.0
  request_parameter_supported: false
  request_uri_parameter_supported: false
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
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  token_endpoint_auth_signing_alg_values_supported:
  - RS256
  - RS384
  - PS256
  type: oauth2
- bearer_format: JWT
  description: The Pixis application backend accepts a bearer JWT minted by the authorization server above. Anonymous requests are rejected by express-jwt with a `credentials_required` error.
  evidence:
    body: '{"error":{"name":"UnauthorizedError","message":"No authorization token was found", "code":"credentials_required","status":401,"inner":{"message":"No authorization token was found"}}}'
    content_type: application/json; charset=utf-8
    request: GET https://core-performance.pixis.ai/ (no Authorization header)
    status: 401
  id: bearer_jwt_application_api
  note: This is the first-party backend for the Pixis web application, not a documented developer API. It is recorded because it is the only live, callable Pixis API host found and it states its own auth requirement plainly. No public reference or spec describes it.
  observed_on: https://core-performance.pixis.ai/
  public: false
  scheme: bearer
  type: http
slug: pixis-authentication
source_filename: pixis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://auth.pixis.ai/.well-known/openid-configuration\nname: Pixis — authentication profile\ndescription: >-\n  Pixis publishes no public developer API and issues no public API keys. What it does publish,\n  machine-readably, is an OpenID Connect / OAuth 2.0 discovery document at auth.pixis.ai — the\n  Auth0 custom domain behind application login for Prism and the Pixis platform. The profile\n  below is read verbatim from that document plus the Auth0Provider configuration Pixis ships in\n  its own public Prism JavaScript bundle, and confirmed against the 401 an anonymous caller gets\n  from the Pixis application backend.\n\nscope_of_this_artifact: >-\n  Application login for Pixis customers. This is NOT a developer-facing API authentication\n  scheme — there is no published token flow for third-party integrators, no client registration\n  a developer can self-serve, and no API reference to authenticate against.\n\nauthorization_server:\n\
  \  issuer: https://auth.pixis.ai/\n  platform: Auth0 (custom domain)\n  discovery:\n    openid_configuration: https://auth.pixis.ai/.well-known/openid-configuration\n    oauth_authorization_server: https://auth.pixis.ai/.well-known/oauth-authorization-server\n    jwks_uri: https://auth.pixis.ai/.well-known/jwks.json\n  endpoints:\n    authorization: https://auth.pixis.ai/authorize\n    token: https://auth.pixis.ai/oauth/token\n    userinfo: https://auth.pixis.ai/userinfo\n    revocation: https://auth.pixis.ai/oauth/revoke\n    device_authorization: https://auth.pixis.ai/oauth/device/code\n    registration: https://auth.pixis.ai/oidc/register\n    mfa_challenge: https://auth.pixis.ai/mfa/challenge\n\nschemes:\n\n  - id: oauth2_oidc\n    type: oauth2\n    protocol: OpenID Connect 1.0 / OAuth 2.0\n    description: >-\n      Authorization Code with PKCE is the flow the Pixis Prism SPA uses; the discovery document\n      also advertises client_credentials, device_code, token-exchange and jwt-bearer.\n\
  \    grant_types_supported:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - implicit\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - http://auth0.com/oauth/grant-type/password-realm\n      - http://auth0.com/oauth/grant-type/passwordless/otp\n      - http://auth0.com/oauth/grant-type/mfa-oob\n      - http://auth0.com/oauth/grant-type/mfa-otp\n      - http://auth0.com/oauth/grant-type/mfa-recovery-code\n    pkce:\n      supported: true\n      code_challenge_methods: [S256, plain]\n    response_types_supported:\n      - code\n      - token\n      - id_token\n      - code token\n      - code id_token\n      - token id_token\n      - code token id_token\n    response_modes_supported: [query, fragment, form_post]\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n\
  \      - private_key_jwt\n      - none\n    token_endpoint_auth_signing_alg_values_supported: [RS256, RS384, PS256]\n    id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n    dpop_signing_alg_values_supported: [ES256]\n    subject_types_supported: [public]\n    dynamic_client_registration:\n      endpoint: https://auth.pixis.ai/oidc/register\n      note: >-\n        Advertised by the discovery document. Auth0 gates this behind a per-tenant toggle;\n        not probed with a write request.\n    request_parameter_supported: false\n    request_uri_parameter_supported: false\n    mfa:\n      supported: true\n      evidence: mfa_challenge_endpoint plus four mfa-* grant types in the discovery document.\n\n  - id: bearer_jwt_application_api\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: >-\n      The Pixis application backend accepts a bearer JWT minted by the authorization server\n      above. Anonymous requests are rejected by express-jwt with a `credentials_required`\
  \ error.\n    observed_on: https://core-performance.pixis.ai/\n    evidence:\n      request: GET https://core-performance.pixis.ai/ (no Authorization header)\n      status: 401\n      content_type: application/json; charset=utf-8\n      body: >-\n        {\"error\":{\"name\":\"UnauthorizedError\",\"message\":\"No authorization token was found\",\n        \"code\":\"credentials_required\",\"status\":401,\"inner\":{\"message\":\"No authorization token was found\"}}}\n    public: false\n    note: >-\n      This is the first-party backend for the Pixis web application, not a documented developer\n      API. It is recorded because it is the only live, callable Pixis API host found and it\n      states its own auth requirement plainly. No public reference or spec describes it.\n\nclient_configuration_observed:\n  source: https://prism.pixis.ai/assets/index-Bof3QprB.js\n  note: >-\n    Pixis ships its Auth0 SPA configuration in a public, unminified-enough bundle. Values below\n    are public-by-design\
  \ SPA client parameters, not secrets.\n  domain: auth.pixis.ai\n  audience: https://cross-platform-prod.us.auth0.com/api/v2/\n  scopes_requested: [openid, profile, email, offline_access]\n  cache_location: localstorage\n  use_refresh_tokens: true\n\napi_keys:\n  supported: false\n  note: >-\n    No API key issuance, key prefix, key management screen, or key documentation was found on\n    any Pixis public surface.\n\nmtls:\n  supported: false\n\ngaps:\n  - No public developer authentication documentation.\n  - No OAuth scopes documented for a Pixis API — the scopes_supported list is the stock Auth0\n    OIDC profile-claim set, not a Pixis resource permission model.\n  - No /.well-known/oauth-protected-resource (RFC 9728) on any host, so an agent cannot discover\n    which resource server the authorization server protects.\n  - No security.txt on any host, including auth.pixis.ai.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixis/refs/heads/main/authentication/pixis-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Enterprise
- Advertising
- Marketing
- Artificial Intelligence
- Generative AI
- Advertising Technology
- Marketing Automation
---
