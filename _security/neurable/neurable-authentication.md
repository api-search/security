---
api_key_in: []
api_specs:
- filename: neurable-core-api-openapi.yml
  format: yaml
  label: Neurable Core API
  slug: neurable-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-core-api-openapi.yml
- filename: neurable-oauth-api-openapi.yml
  format: yaml
  label: Neurable O Auth API
  slug: neurable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-oauth-api-openapi.yml
- filename: neurable-oidc-api-openapi.yml
  format: yaml
  label: Neurable OIDC API
  slug: neurable-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-oidc-api-openapi.yml
- filename: neurable-open-api-openapi.yml
  format: yaml
  label: Neurable Open API
  slug: neurable-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-open-api-openapi.yml
- filename: neurable-protected-api-openapi.yml
  format: yaml
  label: Neurable Protected API
  slug: neurable-protected-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-protected-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Neurable Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Neurable secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Neurable
provider_slug: neurable
scheme_count: 2
schemes:
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - email
  description: The pipe service is the Neurable identity provider. It advertises OIDC Discovery metadata with an issuer of https://pipe.neurable.com, RS256-signed ID tokens, and the standard iss/sub/aud/exp/iat/nonce/email claims. claims_parameter_supported is false.
  endpoints:
    authorization_endpoint: https://pipe.neurable.com/oauth/authorize
    jwks_uri: https://pipe.neurable.com/.well-known/jwks.json
    token_endpoint: https://pipe.neurable.com/oauth/token
    userinfo_endpoint: https://pipe.neurable.com/oidc/userinfo
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://pipe.neurable.com
  name: openIdConnect
  openIdConnectUrl: https://pipe.neurable.com/.well-known/openid-configuration
  sources:
  - well-known/neurable-pipe-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
- description: OAuth 2.0 authorization server co-located with the OIDC provider. The /oauth/authorize operation makes code_challenge and code_challenge_method REQUIRED query parameters, so PKCE is mandatory on the authorization-code flow, and it also requires an explicit `audience` parameter (RFC 8707-style resource targeting). Public clients are supported — token_endpoint_auth_methods_supported includes "none" alongside client_secret_post.
  flows:
  - authorization_endpoint: https://pipe.neurable.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    pkce_required: true
    required_parameters:
    - client_id
    - redirect_uri
    - response_type
    - code_challenge
    - code_challenge_method
    - scope
    - audience
    scopes:
    - demos:all:read
    - demos:prime:read
    - session:stream:create
    - openid
    - email
    token_endpoint: https://pipe.neurable.com/oauth/token
  - flow: clientCredentials
    note: Advertised in grant_types_supported. The token endpoint's request body schema (Body_post_oauth_token_oauth_token_post) is served as application/x-www-form-urlencoded.
    token_endpoint: https://pipe.neurable.com/oauth/token
  - flow: refreshToken
    note: refresh_token appears in grant_types_supported.
    token_endpoint: https://pipe.neurable.com/oauth/token
  name: oauth2
  response_types_supported:
  - code
  sources:
  - well-known/neurable-pipe-openid-configuration.json
  - openapi/neurable-pipe-service-openapi.yml
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  type: oauth2
slug: neurable-authentication
source_filename: neurable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://pipe.neurable.com/.well-known/openid-configuration (HTTP 200) + https://pipe.neurable.com/.well-known/jwks.json (HTTP 200) + openapi/_original/neurable-pipe-openapi.json\ndocs: null\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  api_key_in: []\n  spec_declares_security_schemes: false\nnotes: >-\n  Neurable publishes no public authentication documentation. This profile was probed live: the\n  pipe service at pipe.neurable.com serves a complete OpenID Connect Discovery document and a\n  JWKS, and its own OpenAPI describes the /oauth/authorize, /oauth/token, /oidc/userinfo and\n  /.well-known/jwks.json operations. IMPORTANT GAP — none of the three published Neurable\n  OpenAPI documents declares a components.securitySchemes block, and no operation carries a\n  security requirement, even though the Analytics Service tags five of its six operations\n  \"\
  protected\". The auth model therefore has to be inferred from the discovery document rather\n  than read off the contract.\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://pipe.neurable.com/.well-known/openid-configuration\n  issuer: https://pipe.neurable.com\n  description: >-\n    The pipe service is the Neurable identity provider. It advertises OIDC Discovery metadata\n    with an issuer of https://pipe.neurable.com, RS256-signed ID tokens, and the standard\n    iss/sub/aud/exp/iat/nonce/email claims. claims_parameter_supported is false.\n  endpoints:\n    authorization_endpoint: https://pipe.neurable.com/oauth/authorize\n    token_endpoint: https://pipe.neurable.com/oauth/token\n    userinfo_endpoint: https://pipe.neurable.com/oidc/userinfo\n    jwks_uri: https://pipe.neurable.com/.well-known/jwks.json\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  -\
  \ exp\n  - iat\n  - nonce\n  - email\n  sources:\n  - well-known/neurable-pipe-openid-configuration.json\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization server co-located with the OIDC provider. The /oauth/authorize\n    operation makes code_challenge and code_challenge_method REQUIRED query parameters, so PKCE\n    is mandatory on the authorization-code flow, and it also requires an explicit `audience`\n    parameter (RFC 8707-style resource targeting). Public clients are supported —\n    token_endpoint_auth_methods_supported includes \"none\" alongside client_secret_post.\n  flows:\n  - flow: authorizationCode\n    authorization_endpoint: https://pipe.neurable.com/oauth/authorize\n    token_endpoint: https://pipe.neurable.com/oauth/token\n    pkce: S256\n    pkce_required: true\n    required_parameters:\n    - client_id\n    - redirect_uri\n    - response_type\n    - code_challenge\n    - code_challenge_method\n    - scope\n    - audience\n    scopes:\n\
  \    - demos:all:read\n    - demos:prime:read\n    - session:stream:create\n    - openid\n    - email\n  - flow: clientCredentials\n    token_endpoint: https://pipe.neurable.com/oauth/token\n    note: >-\n      Advertised in grant_types_supported. The token endpoint's request body schema\n      (Body_post_oauth_token_oauth_token_post) is served as\n      application/x-www-form-urlencoded.\n  - flow: refreshToken\n    token_endpoint: https://pipe.neurable.com/oauth/token\n    note: refresh_token appears in grant_types_supported.\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_post\n  sources:\n  - well-known/neurable-pipe-openid-configuration.json\n  - openapi/neurable-pipe-service-openapi.yml\nunauthenticated_surface:\n- operation: create_headset_license_open_headset_license_post\n  method: POST\n  path: /open/headset/license\n  host: https://analytics-service.neurable.com\n  note: >-\n    Tagged \"open\" (as opposed to the\
  \ \"protected\" tag on every other Analytics Service\n    operation), which is the only in-spec signal that it is reachable without a token. It\n    issues an HMAC-signed HeadsetLicense keyed to a device serial_number + firmware_uuid; the\n    documented error enum (SERIAL_NUMBER_UNAUTHORIZED, SERIAL_NUMBER_ALREADY_ISSUED) shows\n    authorization is enforced on the serial number rather than on a caller credential.\n  probed: not exercised — no request was sent to this endpoint.\ncross_links:\n  scopes: scopes/neurable-scopes.yml\n  conventions: conventions/neurable-conventions.yml\n  conformance: conformance/neurable-conformance.yml\n  well_known: well-known/neurable-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/authentication/neurable-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- neurotechnology
- brain-computer-interface
- eeg
- neuroscience
- wearables
- biosignals
- hardware
- consumer-electronics
- research-tools
- cognitive-analytics
- health-data
- Authentication
- openid-connect
---
