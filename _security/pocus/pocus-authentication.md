---
api_key_in: []
auth_types: []
description: Pocus runs a standards-based OAuth 2.0 authorization server and OpenID Connect provider at auth.pocus.com and publishes its metadata anonymously. Enterprise identity federates in over SAML 2.0 (Okta documented) with SCIM 2.0 provisioning. The core GraphQL API at api.pocus.com accepts a bearer JWT. Pocus publishes no OpenAPI, so no securityScheme could be derived from a contract — everything below is read from documents the provider actually serves.
kind: authentication
layout: security
method: probed
name: Pocus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pocus declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Pocus
provider_slug: pocus
scheme_count: 5
schemes:
- client_authentication:
  - client_secret_basic
  - client_secret_post
  description: OAuth 2.0 authorization server at https://auth.pocus.com, advertised via RFC 8414 authorization-server metadata.
  endpoints:
    authorization: https://auth.pocus.com/oauth/authorize
    device_authorization: https://auth.pocus.com/oauth/device/authorize
    end_session: https://auth.pocus.com/oauth/logout
    jwks: https://auth.pocus.com/.well-known/jwks.json
    token: https://auth.pocus.com/oauth/token
    userinfo: https://auth.pocus.com/identity/resources/users/v2/me
  evidence:
    status: 200
    url: https://auth.pocus.com/.well-known/oauth-authorization-server
  flows:
  - code_challenge_methods:
    - S256
    grant: authorization_code
    pkce: true
    response_modes:
    - query
    response_types:
    - code
  - grant: refresh_token
  - grant: client_credentials
  - grant: urn:ietf:params:oauth:grant-type:token-exchange
    rfc: RFC 8693
  - grant: urn:ietf:params:oauth:grant-type:device_code
    rfc: RFC 8628
  id: pocus_oauth2
  issuer: https://auth.pocus.com
  scopes:
  - openid
  - profile
  - email
  type: oauth2
- description: OpenID Connect provider co-located on the same issuer.
  evidence:
    status: 200
    url: https://auth.pocus.com/.well-known/openid-configuration
  id: pocus_oidc
  id_token_signing_alg_values_supported:
  - RS256
  - ES256
  jwks_status: HTTP 200 — one RSA signing key, kid b936d5e7, alg RS256, use sig
  openIdConnectUrl: https://auth.pocus.com/.well-known/openid-configuration
  subject_types_supported:
  - public
  token_endpoint_auth_signing_alg_values_supported:
  - RS256
  - ES256
  type: openIdConnect
- applies_to: https://api.pocus.com/graphql
  bearerFormat: JWT
  description: 'The core GraphQL API at https://api.pocus.com/graphql is called with `Authorization: Bearer <JWT>`.'
  evidence: Read from Pocus' own published @pocus/cli 0.1.1 (lib/util/graphqlClient.js), which sets headers.Authorization to `Bearer ${...getIdToken().getJwtToken()}` against `${POCUS_CORE_API_ENDPOINT}/graphql`.
  id: pocus_bearer_jwt
  note: The published CLI obtained that JWT from an AWS Cognito user pool that no longer exists; current tokens are issued by auth.pocus.com. The CLI is 2021-era and is not a current description of how a caller should authenticate.
  scheme: bearer
  type: http
- acs_url: https://auth.pocus.com/auth/saml/callback
  audience_uri: pocus
  configured_in: Workspace Settings > User Management > SSO > Setup SSO Connection
  description: SAML 2.0 single sign-on for enterprise workspaces; Okta is the documented IdP.
  evidence:
    status: 200
    url: https://docs.pocus.com/docs/okta
  group_mapping: Okta groups map to Pocus roles (see https://docs.pocus.com/docs/permissions). Custom Okta user attributes are pulled at login.
  id: pocus_saml_sso
  type: saml2
- base_url: null
  base_url_note: The SCIM base URL is tenant-issued and only visible inside an authenticated Pocus workspace; Pocus does not publish it, so it is recorded as null rather than guessed.
  description: SCIM 2.0 provisioning connector. Pocus issues a per-connection provisioning URL (the "SCIM connector base URL") and an authorization token; Okta is configured with authentication mode "HTTP Header" using that token.
  evidence:
    status: 200
    url: https://docs.pocus.com/docs/okta-scim
  id: pocus_scim_token
  scheme: bearer
  type: http
  unique_identifier_field: userName
slug: pocus-authentication
source_filename: pocus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://auth.pocus.com/.well-known/openid-configuration and\n  https://auth.pocus.com/.well-known/oauth-authorization-server (both HTTP 200, fetched\n  2026-08-26); https://docs.pocus.com/docs/okta and /docs/okta-scim; the published @pocus/cli\n  0.1.1 package source\ndocs: https://docs.pocus.com/docs/okta\nname: Pocus authentication profile\ndescription: >-\n  Pocus runs a standards-based OAuth 2.0 authorization server and OpenID Connect provider at\n  auth.pocus.com and publishes its metadata anonymously. Enterprise identity federates in over\n  SAML 2.0 (Okta documented) with SCIM 2.0 provisioning. The core GraphQL API at api.pocus.com\n  accepts a bearer JWT. Pocus publishes no OpenAPI, so no securityScheme could be derived from a\n  contract — everything below is read from documents the provider actually serves.\n\nschemes:\n- id: pocus_oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization server at\
  \ https://auth.pocus.com, advertised via RFC 8414\n    authorization-server metadata.\n  issuer: https://auth.pocus.com\n  endpoints:\n    authorization: https://auth.pocus.com/oauth/authorize\n    token: https://auth.pocus.com/oauth/token\n    userinfo: https://auth.pocus.com/identity/resources/users/v2/me\n    jwks: https://auth.pocus.com/.well-known/jwks.json\n    end_session: https://auth.pocus.com/oauth/logout\n    device_authorization: https://auth.pocus.com/oauth/device/authorize\n  flows:\n  - grant: authorization_code\n    pkce: true\n    code_challenge_methods: [S256]\n    response_types: [code]\n    response_modes: [query]\n  - grant: refresh_token\n  - grant: client_credentials\n  - grant: 'urn:ietf:params:oauth:grant-type:token-exchange'\n    rfc: RFC 8693\n  - grant: 'urn:ietf:params:oauth:grant-type:device_code'\n    rfc: RFC 8628\n  client_authentication: [client_secret_basic, client_secret_post]\n  scopes: [openid, profile, email]\n  evidence:\n    url: https://auth.pocus.com/.well-known/oauth-authorization-server\n\
  \    status: 200\n\n- id: pocus_oidc\n  type: openIdConnect\n  description: OpenID Connect provider co-located on the same issuer.\n  openIdConnectUrl: https://auth.pocus.com/.well-known/openid-configuration\n  subject_types_supported: [public]\n  id_token_signing_alg_values_supported: [RS256, ES256]\n  token_endpoint_auth_signing_alg_values_supported: [RS256, ES256]\n  jwks_status: 'HTTP 200 — one RSA signing key, kid b936d5e7, alg RS256, use sig'\n  evidence:\n    url: https://auth.pocus.com/.well-known/openid-configuration\n    status: 200\n\n- id: pocus_bearer_jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    The core GraphQL API at https://api.pocus.com/graphql is called with\n    `Authorization: Bearer <JWT>`.\n  applies_to: https://api.pocus.com/graphql\n  evidence: >-\n    Read from Pocus' own published @pocus/cli 0.1.1 (lib/util/graphqlClient.js), which sets\n    headers.Authorization to `Bearer ${...getIdToken().getJwtToken()}` against\n    `${POCUS_CORE_API_ENDPOINT}/graphql`.\n\
  \  note: >-\n    The published CLI obtained that JWT from an AWS Cognito user pool that no longer exists;\n    current tokens are issued by auth.pocus.com. The CLI is 2021-era and is not a current\n    description of how a caller should authenticate.\n\n- id: pocus_saml_sso\n  type: saml2\n  description: SAML 2.0 single sign-on for enterprise workspaces; Okta is the documented IdP.\n  acs_url: https://auth.pocus.com/auth/saml/callback\n  audience_uri: pocus\n  group_mapping: >-\n    Okta groups map to Pocus roles (see https://docs.pocus.com/docs/permissions). Custom Okta user\n    attributes are pulled at login.\n  configured_in: Workspace Settings > User Management > SSO > Setup SSO Connection\n  evidence:\n    url: https://docs.pocus.com/docs/okta\n    status: 200\n\n- id: pocus_scim_token\n  type: http\n  scheme: bearer\n  description: >-\n    SCIM 2.0 provisioning connector. Pocus issues a per-connection provisioning URL (the \"SCIM\n    connector base URL\") and an authorization token;\
  \ Okta is configured with authentication mode\n    \"HTTP Header\" using that token.\n  unique_identifier_field: userName\n  base_url: null\n  base_url_note: >-\n    The SCIM base URL is tenant-issued and only visible inside an authenticated Pocus workspace;\n    Pocus does not publish it, so it is recorded as null rather than guessed.\n  evidence:\n    url: https://docs.pocus.com/docs/okta-scim\n    status: 200\n\napi_key_support: false\napi_key_note: >-\n  No public API key programme, key prefix, or self-serve credential issuance was found anywhere on\n  pocus.com or docs.pocus.com. There is no developer signup that yields an API credential.\n\nsummary:\n  schemes_count: 5\n  primary: OAuth 2.0 / OpenID Connect (auth.pocus.com)\n  machine_readable_auth_metadata: true\n  derived_from_openapi: false\n  gap: >-\n    Authentication metadata is excellent and standards-based, but there is no published API\n    reference binding it to operations — a developer can discover how to get a token\
  \ and cannot\n    discover what to call with it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pocus/refs/heads/main/authentication/pocus-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Sales Intelligence
- Product-Led Sales
- Revenue Operations
- Go-To-Market
- Data Enrichment
- CRM
- Artificial Intelligence
- GraphQL
---
