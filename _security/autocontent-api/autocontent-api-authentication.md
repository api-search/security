---
anonymous_access: false
api_key_in: []
api_specs:
- filename: autocontent-api-content-api-openapi.yml
  format: yaml
  label: AutoContent API Content API
  slug: autocontent-api-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-content-api-openapi.yml
- filename: autocontent-api-dedicated-account-api-openapi.yml
  format: yaml
  label: AutoContent API Dedicated Account API
  slug: autocontent-api-dedicated-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-dedicated-account-api-openapi.yml
- filename: autocontent-api-podcast-api-openapi.yml
  format: yaml
  label: AutoContent API Podcast API
  slug: autocontent-api-podcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-podcast-api-openapi.yml
- filename: autocontent-api-share-api-openapi.yml
  format: yaml
  label: AutoContent API Share API
  slug: autocontent-api-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-share-api-openapi.yml
- filename: autocontent-api-video-api-openapi.yml
  format: yaml
  label: AutoContent API Video API
  slug: autocontent-api-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-video-api-openapi.yml
- filename: autocontent-api-platform-v1-openapi.json
  format: json
  label: AutoContent Platform API v1
  slug: platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-platform-v1-openapi.json
- filename: autocontent-api-legacy-content-openapi.json
  format: json
  label: AutoContent legacy Content API
  slug: legacy-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-legacy-content-openapi.json
auth_types:
- http
- oauth2
description: 'Two credential families for two products. The Platform API accepts either a scoped API key (acp_ prefix) or an OAuth access token, both presented as Authorization: Bearer. The legacy Content API takes its own JWT bearer token and shares nothing with the Platform credentials.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Autocontent Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: AutoContent API secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AutoContent API
provider_slug: autocontent-api
scheme_count: 3
schemes:
- bearerFormat: acp_ Platform API key
  guidance: '"Keep the key on the server or in a secret manager; never ship it in browser JavaScript." AUTOCONTENT_API_KEY is the documented environment variable for the SDK and CLI, and the CLI treats it as overriding any locally stored key — the preferred CI/agent path.'
  header: 'Authorization: Bearer <key>'
  key_prefix: acp_
  minted_by: createApiKey (POST /api-keys, scope platform.keys.write) or the Platform app
  name: platformApiKey
  product: AutoContent Platform API v1
  revocable: true
  revoked_by: revokeApiKey (DELETE /api-keys/{id})
  scheme: bearer
  scoped: true
  sources:
  - openapi/autocontent-api-platform-v1-openapi.json
  - https://autocontentapi.com/developers/api
  type: http
- bearerFormat: Platform OAuth JWT
  name: platformOAuth
  note: Public-client OAuth only — token_endpoint_auth_methods_supported is ["none"], so PKCE is the protection, not a client secret. Dynamic client registration at /reg is what lets an arbitrary MCP client obtain a client_id without a human in the loop.
  oauth:
    authorization_endpoint: https://auth.autocontentapi.com/auth
    dynamic_client_registration: true
    end_session_endpoint: https://auth.autocontentapi.com/session/end
    grant_types:
    - authorization_code
    - refresh_token
    issuer: https://auth.autocontentapi.com
    jwks_uri: https://auth.autocontentapi.com/jwks
    pkce:
    - S256
    registration_endpoint: https://auth.autocontentapi.com/reg
    response_types:
    - code
    revocation_endpoint: https://auth.autocontentapi.com/token/revocation
    scopes:
    - platform.read
    - platform.write
    - platform.generate
    - platform.billing.read
    - platform.billing.write
    - platform.keys.write
    token_endpoint: https://auth.autocontentapi.com/token
    token_endpoint_auth_methods:
    - none
  product: AutoContent Platform API v1
  scheme: bearer
  sources:
  - openapi/autocontent-api-platform-v1-openapi.json
  - well-known/autocontent-api-auth-oauth-authorization-server.json
  type: http
- bearerFormat: JWT
  description: Legacy API token, applied as a global security requirement across the legacy Content API. 87 of its 106 operations declare a 401 response.
  header: 'Authorization: Bearer <token>'
  name: bearerAuth
  note: Separate credential space from the Platform. The provider states legacy routes, credentials and credit vocabulary remain separate and are not compatibility aliases for /v1.
  product: AutoContent legacy Content API
  scheme: bearer
  sources:
  - openapi/autocontent-api-legacy-content-openapi.json
  type: http
slug: autocontent-api-authentication
source_filename: autocontent-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://autocontentapi.com/developers/api and https://autocontentapi.com/developers (auth\n  guidance), components.securitySchemes in openapi/autocontent-api-platform-v1-openapi.json and\n  openapi/autocontent-api-legacy-content-openapi.json, and the fetched authorization-server\n  metadata at well-known/autocontent-api-auth-oauth-authorization-server.json.\ndocs: https://autocontentapi.com/developers/api\nsummary:\n  types:\n  - http\n  - oauth2\n  products: 2\ndescription: >-\n  Two credential families for two products. The Platform API accepts either a scoped API key\n  (acp_ prefix) or an OAuth access token, both presented as Authorization: Bearer. The legacy\n  Content API takes its own JWT bearer token and shares nothing with the Platform credentials.\nschemes:\n- name: platformApiKey\n  product: AutoContent Platform API v1\n  type: http\n  scheme: bearer\n  bearerFormat: acp_ Platform API key\n  key_prefix: acp_\n\
  \  scoped: true\n  header: 'Authorization: Bearer <key>'\n  minted_by: createApiKey (POST /api-keys, scope platform.keys.write) or the Platform app\n  revocable: true\n  revoked_by: revokeApiKey (DELETE /api-keys/{id})\n  guidance: >-\n    \"Keep the key on the server or in a secret manager; never ship it in browser JavaScript.\"\n    AUTOCONTENT_API_KEY is the documented environment variable for the SDK and CLI, and the CLI\n    treats it as overriding any locally stored key — the preferred CI/agent path.\n  sources:\n  - openapi/autocontent-api-platform-v1-openapi.json\n  - https://autocontentapi.com/developers/api\n- name: platformOAuth\n  product: AutoContent Platform API v1\n  type: http\n  scheme: bearer\n  bearerFormat: Platform OAuth JWT\n  oauth:\n    issuer: https://auth.autocontentapi.com\n    authorization_endpoint: https://auth.autocontentapi.com/auth\n    token_endpoint: https://auth.autocontentapi.com/token\n    revocation_endpoint: https://auth.autocontentapi.com/token/revocation\n\
  \    registration_endpoint: https://auth.autocontentapi.com/reg\n    jwks_uri: https://auth.autocontentapi.com/jwks\n    end_session_endpoint: https://auth.autocontentapi.com/session/end\n    grant_types:\n    - authorization_code\n    - refresh_token\n    response_types:\n    - code\n    pkce:\n    - S256\n    token_endpoint_auth_methods:\n    - none\n    dynamic_client_registration: true\n    scopes:\n    - platform.read\n    - platform.write\n    - platform.generate\n    - platform.billing.read\n    - platform.billing.write\n    - platform.keys.write\n  note: >-\n    Public-client OAuth only — token_endpoint_auth_methods_supported is [\"none\"], so PKCE is the\n    protection, not a client secret. Dynamic client registration at /reg is what lets an arbitrary\n    MCP client obtain a client_id without a human in the loop.\n  sources:\n  - openapi/autocontent-api-platform-v1-openapi.json\n  - well-known/autocontent-api-auth-oauth-authorization-server.json\n- name: bearerAuth\n  product:\
  \ AutoContent legacy Content API\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer <token>'\n  description: >-\n    Legacy API token, applied as a global security requirement across the legacy Content API. 87 of\n    its 106 operations declare a 401 response.\n  note: >-\n    Separate credential space from the Platform. The provider states legacy routes, credentials and\n    credit vocabulary remain separate and are not compatibility aliases for /v1.\n  sources:\n  - openapi/autocontent-api-legacy-content-openapi.json\nunauthenticated_surface:\n- path: /podcast/ideas\n  spec: openapi/autocontent-api-legacy-content-openapi.json\n  auth: none\n  gate: >-\n    Origin allowlist (autocontentapi.com / app.autocontentapi.com / localhost) OR a\n    X-Free-Tools-Secret header; other callers get 403. Limits 2 requests per IP per 24h, 30 total\n    per 24h, 2 concurrent per IP.\n  note: >-\n    The only route on either surface that runs without a credential. It\
  \ is origin-gated, not open.\nmfa: null\nmtls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/authentication/autocontent-api-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Artificial Intelligence
- Audio
- Content Generation
- Podcasts
- Video
- Generative AI
- Text-to-Speech
- Automation
---
