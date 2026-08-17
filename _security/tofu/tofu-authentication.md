---
api_key_in:
- header
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Tofu Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
overview: Tofu secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, and deviceCode flow(s).
provider_name: Tofu
provider_slug: tofu
scheme_count: 3
schemes:
- acquisition:
    method: emailed one-time code
    note: There is no self-serve developer console or key-management page. The key is issued to and stored by the CLI (~/.config/enrich/config.json); it can be overridden with the ENRICH_API_KEY environment variable.
    steps:
    - enrich signup <email> — a 6-digit code is emailed
    - enrich verify <code> — exchanges the code for a key the CLI stores
  applies_to: https://api.enrich.tofuhq.com
  evidence: 'An unauthenticated request returns HTTP 401 with {"error":{"code":"unauthorized","message":"missing or malformed API key (expected \"Authorization: Bearer enr_...\")"}} — the API states its own key prefix and header in the error body.'
  format: Bearer enr_<key>
  header: Authorization
  in: header
  key_prefix: enr_
  name: EnrichBearerKey
  scheme: bearer
  sources:
  - live probe of https://api.enrich.tofuhq.com/v1/billing/plans
  type: http
  unauthenticated_endpoints:
  - GET /v1/schema/company
  - GET /v1/schema/person
  - GET /
- applies_to: https://login.tofuhq.com
  endpoints:
    authorization: https://login.tofuhq.com/oauth2/authorize
    device_authorization: https://login.tofuhq.com/oauth2/device_authorization
    introspection: https://login.tofuhq.com/oauth2/introspection
    jwks: https://login.tofuhq.com/oauth2/jwks
    token: https://login.tofuhq.com/oauth2/token
    userinfo: https://login.tofuhq.com/oauth2/userinfo
  id_token_signing_alg:
  - RS256
  issuer: https://login.tofuhq.com
  name: TofuOIDC
  note: This is the Tofu application sign-in authorization server (the surface behind login.tofuhq.com / app.tofuhq.com), not the auth mechanism for the Enrich API.
  openIdConnectUrl: https://login.tofuhq.com/.well-known/openid-configuration
  sources:
  - well-known/tofu-openid-configuration.json
  subject_types:
  - public
  type: openIdConnect
- applies_to: https://login.tofuhq.com
  flows:
  - authorizationUrl: https://login.tofuhq.com/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    scopes:
    - openid
    - profile
    - email
    - offline_access
    tokenUrl: https://login.tofuhq.com/oauth2/token
  - flow: refreshToken
    tokenUrl: https://login.tofuhq.com/oauth2/token
  - deviceAuthorizationUrl: https://login.tofuhq.com/oauth2/device_authorization
    flow: deviceCode
    grant: urn:ietf:params:oauth:grant-type:device_code
    tokenUrl: https://login.tofuhq.com/oauth2/token
  - flow: clientCredentials
    note: Advertised in openid-configuration `grant_types_supported` but NOT in the RFC 8414 oauth-authorization-server document. Recorded as-published; the divergence between the two discovery documents is the provider's.
    tokenUrl: https://login.tofuhq.com/oauth2/token
  name: TofuOAuth2
  response_modes:
  - query
  response_types:
  - code
  sources:
  - well-known/tofu-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: tofu-authentication
source_filename: tofu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live probes of api.enrich.tofuhq.com and login.tofuhq.com/.well-known/*\ndocs: https://enrich.tofuhq.com\nsummary:\n  types: [http, oauth2, openIdConnect]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, deviceCode]\n  openapi_available: false\nschemes:\n- name: EnrichBearerKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Bearer enr_<key>\"\n  applies_to: https://api.enrich.tofuhq.com\n  sources: [live probe of https://api.enrich.tofuhq.com/v1/billing/plans]\n  evidence: >-\n    An unauthenticated request returns HTTP 401 with\n    {\"error\":{\"code\":\"unauthorized\",\"message\":\"missing or malformed API key\n    (expected \\\"Authorization: Bearer enr_...\\\")\"}} — the API states its own key\n    prefix and header in the error body.\n  key_prefix: enr_\n  acquisition:\n    method: emailed one-time code\n    steps:\n\
  \    - \"enrich signup <email> — a 6-digit code is emailed\"\n    - \"enrich verify <code> — exchanges the code for a key the CLI stores\"\n    note: >-\n      There is no self-serve developer console or key-management page. The key is\n      issued to and stored by the CLI (~/.config/enrich/config.json); it can be\n      overridden with the ENRICH_API_KEY environment variable.\n  unauthenticated_endpoints:\n  - GET /v1/schema/company\n  - GET /v1/schema/person\n  - GET /\n- name: TofuOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://login.tofuhq.com/.well-known/openid-configuration\n  applies_to: https://login.tofuhq.com\n  issuer: https://login.tofuhq.com\n  sources: [well-known/tofu-openid-configuration.json]\n  endpoints:\n    authorization: https://login.tofuhq.com/oauth2/authorize\n    token: https://login.tofuhq.com/oauth2/token\n    userinfo: https://login.tofuhq.com/oauth2/userinfo\n    introspection: https://login.tofuhq.com/oauth2/introspection\n    device_authorization:\
  \ https://login.tofuhq.com/oauth2/device_authorization\n    jwks: https://login.tofuhq.com/oauth2/jwks\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\n  note: >-\n    This is the Tofu application sign-in authorization server (the surface behind\n    login.tofuhq.com / app.tofuhq.com), not the auth mechanism for the Enrich API.\n- name: TofuOAuth2\n  type: oauth2\n  applies_to: https://login.tofuhq.com\n  sources: [well-known/tofu-oauth-authorization-server.json]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tofuhq.com/oauth2/authorize\n    tokenUrl: https://login.tofuhq.com/oauth2/token\n    pkce: [S256]\n    scopes: [openid, profile, email, offline_access]\n  - flow: refreshToken\n    tokenUrl: https://login.tofuhq.com/oauth2/token\n  - flow: deviceCode\n    grant: urn:ietf:params:oauth:grant-type:device_code\n    deviceAuthorizationUrl: https://login.tofuhq.com/oauth2/device_authorization\n    tokenUrl: https://login.tofuhq.com/oauth2/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://login.tofuhq.com/oauth2/token\n    note: >-\n      Advertised in openid-configuration `grant_types_supported` but NOT in the\n      RFC 8414 oauth-authorization-server document. Recorded as-published; the\n      divergence between the two discovery documents is the provider's.\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  response_types: [code]\n  response_modes: [query]\nnotes: >-\n  Two distinct authentication surfaces on the same domain, and they do not share a\n  mechanism. The Enrich API (api.enrich.tofuhq.com) is a bearer API key with an\n  `enr_` prefix, provisioned by email code through the CLI. The application login\n  (login.tofuhq.com) is a full OAuth 2.0 / OIDC authorization server with PKCE and\n  device-code support. Neither the OIDC issuer nor its scopes govern the Enrich\n  API; api.enrich.tofuhq.com returns 404 for\n  /.well-known/oauth-protected-resource, so the two are not linked\
  \ by discovery.\n  No OpenAPI is published, so nothing here is derived from a spec — every scheme\n  was read from a live document or a live error response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tofu/refs/heads/main/authentication/tofu-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Ai Ml
- Marketing
- Go-To-Market
- Sales
- Automation
- CRM
- Campaigns
- Data Enrichment
- Company Data
- People Data
- Lead Generation
- Agents
- Contact Data
---
