---
anonymous_access: false
api_key_in: []
api_specs:
- filename: authologic-aml-api-openapi.yml
  format: yaml
  label: Authologic AML API
  slug: authologic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-aml-api-openapi.yml
- filename: authologic-advanced-api-openapi.yml
  format: yaml
  label: Authologic Advanced API
  slug: authologic-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-advanced-api-openapi.yml
- filename: authologic-affordability-assessment-api-openapi.yml
  format: yaml
  label: Authologic Affordability assessment API
  slug: authologic-affordability-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-affordability-assessment-api-openapi.yml
- filename: authologic-aml-api-openapi.yml
  format: yaml
  label: Authologic AML API
  slug: authologic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-aml-api-openapi.yml
- filename: authologic-bank-api-openapi.yml
  format: yaml
  label: Authologic Bank API
  slug: authologic-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-bank-api-openapi.yml
- filename: authologic-conversation-api-openapi.yml
  format: yaml
  label: Authologic Conversation API
  slug: authologic-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-conversation-api-openapi.yml
- filename: authologic-database-verification-api-openapi.yml
  format: yaml
  label: Authologic Database Verification API
  slug: authologic-database-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-database-verification-api-openapi.yml
- filename: authologic-enterprise-integration-api-openapi.yml
  format: yaml
  label: Authologic Enterprise Integration API
  slug: authologic-enterprise-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-enterprise-integration-api-openapi.yml
- filename: authologic-metadata-api-openapi.yml
  format: yaml
  label: Authologic Metadata API
  slug: authologic-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-metadata-api-openapi.yml
auth_types:
- http
- oauth2
description: Authologic offers two authentication styles over the same credential pair, and the published OAuth authorization server is materially richer than the OpenAPI lets on. The spec declares one clientCredentials flow; the RFC 8414 metadata document advertises five grant types, mTLS-bound tokens and DPoP.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Authologic Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Authologic secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Authologic
provider_slug: authologic
scheme_count: 2
schemes:
- credential_scope: per environment (a sandbox key does not work against production)
  description: Username is the account name; password is the environment-specific API key. This is the style every published example uses (`curl -u my_login`). The key is generated in the API Keys section of OmniPanel and is NOT the OmniPanel account password — the docs call the confusion out explicitly.
  issuance: https://omnipanel.authologic.com
  label: HTTP Basic
  name: apiKey
  rotation: Self-serve — generate a new key in OmniPanel. No rotation policy or key lifetime is published, and no expiry is signalled at runtime.
  scheme: basic
  sources:
  - openapi/authologic-customer-api-openapi.yml
  - https://developer.authologic.com/docs/technical/implementation
  type: http
  verified:
    date: '2026-09-14'
    header: 'www-authenticate: Basic realm="Realm"'
    probe: POST https://sandbox.authologic.com/api/conversations
    status: 401
- description: 'The same account name and API key are used as client_id and client_secret. POST to the token endpoint with Content-Type application/x-www-form-urlencoded and grant_type=client_credentials, then send Authorization: Bearer <token> on subsequent calls.'
  flows:
  - flow: clientCredentials
    scopes: 0
    scopes_note: The scopes object is EMPTY in the contract and no scope taxonomy is published anywhere. Authorization is account- and environment-scoped, not scope-scoped. See scopes/authologic-scopes.yml.
    tokenUrl: https://sandbox.authologic.com/api/oauth2/token
  label: OAuth 2.0 client credentials
  name: oauth2
  sources:
  - openapi/authologic-customer-api-openapi.yml
  token_lifetime: not published
  token_type: Bearer
  type: oauth2
slug: authologic-authentication
source_filename: authologic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://developer.authologic.com/docs/technical/implementation,\n  openapi/authologic-customer-api-openapi.yml (components.securitySchemes),\n  well-known/authologic-sandbox-oauth-authorization-server.json (RFC 8414, probed 2026-09-14),\n  live 401 probe of https://sandbox.authologic.com/api/conversations\ndocs: https://developer.authologic.com/docs/technical/implementation\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Authologic\nproviderId: authologic\ndescription: >-\n  Authologic offers two authentication styles over the same credential pair, and the published OAuth\n  authorization server is materially richer than the OpenAPI lets on. The spec declares one\n  clientCredentials flow; the RFC 8414 metadata document advertises five grant types, mTLS-bound tokens\n  and DPoP.\nsummary:\n  types:\n    - http\n    - oauth2\n  oauth2_flows:\n    - clientCredentials\n  default_security: 'either\
  \ scheme satisfies the requirement — security: [{apiKey: []}, {oauth2: []}]'\n  applies_to: all 14 operations\n  transport: HTTPS only\nschemes:\n  - name: apiKey\n    type: http\n    scheme: basic\n    label: HTTP Basic\n    description: >-\n      Username is the account name; password is the environment-specific API key. This is the style every\n      published example uses (`curl -u my_login`). The key is generated in the API Keys section of\n      OmniPanel and is NOT the OmniPanel account password — the docs call the confusion out explicitly.\n    credential_scope: per environment (a sandbox key does not work against production)\n    issuance: https://omnipanel.authologic.com\n    rotation: >-\n      Self-serve — generate a new key in OmniPanel. No rotation policy or key lifetime is published, and\n      no expiry is signalled at runtime.\n    verified:\n      probe: POST https://sandbox.authologic.com/api/conversations\n      status: 401\n      header: 'www-authenticate: Basic realm=\"\
  Realm\"'\n      date: '2026-09-14'\n    sources:\n      - openapi/authologic-customer-api-openapi.yml\n      - https://developer.authologic.com/docs/technical/implementation\n  - name: oauth2\n    type: oauth2\n    label: OAuth 2.0 client credentials\n    description: >-\n      The same account name and API key are used as client_id and client_secret. POST to the token\n      endpoint with Content-Type application/x-www-form-urlencoded and grant_type=client_credentials, then\n      send Authorization: Bearer <token> on subsequent calls.\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://sandbox.authologic.com/api/oauth2/token\n        scopes: 0\n        scopes_note: >-\n          The scopes object is EMPTY in the contract and no scope taxonomy is published anywhere.\n          Authorization is account- and environment-scoped, not scope-scoped. See\n          scopes/authologic-scopes.yml.\n    token_type: Bearer\n    token_lifetime: not published\n    sources:\n   \
  \   - openapi/authologic-customer-api-openapi.yml\nauthorization_server:\n  metadata_url: https://sandbox.authologic.com/.well-known/oauth-authorization-server\n  rfc: RFC 8414\n  status: 200\n  probed: '2026-09-14'\n  file: well-known/authologic-sandbox-oauth-authorization-server.json\n  issuer: https://sandbox.authologic.com\n  endpoints:\n    authorization: https://sandbox.authologic.com/oauth2/authorize\n    device_authorization: https://sandbox.authologic.com/oauth2/device_authorization\n    token: https://sandbox.authologic.com/api/oauth2/token\n    jwks: https://sandbox.authologic.com/api/oauth2/jwks\n    introspection: https://sandbox.authologic.com/oauth2/introspect\n    revocation: https://sandbox.authologic.com/oauth2/revoke\n  grant_types_supported:\n    - authorization_code\n    - client_credentials\n    - refresh_token\n    - 'urn:ietf:params:oauth:grant-type:device_code'\n    - 'urn:ietf:params:oauth:grant-type:token-exchange'\n  response_types_supported:\n    - code\n \
  \ token_endpoint_auth_methods_supported:\n    - client_secret_basic\n    - client_secret_post\n    - client_secret_jwt\n    - private_key_jwt\n    - tls_client_auth\n    - self_signed_tls_client_auth\n  code_challenge_methods_supported:\n    - S256\n  tls_client_certificate_bound_access_tokens: true\n  dpop_signing_alg_values_supported:\n    - RS256\n    - RS384\n    - RS512\n    - PS256\n    - PS384\n    - PS512\n    - ES256\n    - ES384\n    - ES512\n  finding: >-\n    A significant undocumented capability gap. The developer documentation describes Basic auth only and\n    the OpenAPI declares only clientCredentials, yet the environment advertises authorization_code with\n    PKCE, refresh tokens, the device grant, token exchange, private_key_jwt, mutual-TLS client\n    authentication with certificate-bound access tokens (RFC 8705) and DPoP (RFC 9449). For an agent\n    integrator that is the difference between a shared static secret and a cryptographically bound\n    workload credential\
  \ — and nothing in the docs mentions it is available.\nwebhook_authentication:\n  direction: inbound (Authologic to integrator)\n  scheme: HMAC-SHA-256\n  headers:\n    - X-Signature\n    - X-Signature-Timestamp\n  key: >-\n    A dedicated signature key issued by Authologic, distinct from the API key. Replaced at go-live along\n    with the API address and API key.\n  replay_window_minutes: 5\n  detail: asyncapi/authologic-callbacks-webhooks.yml\ngaps:\n  - No OpenID Connect discovery document (/.well-known/openid-configuration returns 404 on every host).\n  - No /.well-known/oauth-protected-resource (RFC 9728), so an MCP-style client cannot discover the\n    authorization server from the resource.\n  - No published token lifetime, no key-rotation policy and no runtime expiry signal for API keys.\n  - >-\n    Production (api.authologic.com) adds an IP allowlist on top of credentials — an unlisted caller never\n    reaches the auth layer and receives an nginx 403 HTML page instead of a\
  \ JSON error.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/authentication/authologic-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- AML
- Digital Identity
- eID
- Identity Verification
- KYB
- KYC
- Liveness Check
---
