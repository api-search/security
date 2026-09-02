---
api_key_in:
- header
api_specs:
- filename: closedloop-public-api-openapi.yaml
  format: yaml
  label: ClosedLoop AI REST API
  slug: closedloop-ai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-public-api-openapi.yaml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Closedloop Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClosedLoop AI secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClosedLoop AI
provider_slug: closedloop
scheme_count: 3
schemes:
- alias_parameter: apikey
  description: 'Team-scoped API key created in the app (Settings → API Keys).

    Sent as `X-API-Key: <key>` on every request. The header name `apikey`

    is also accepted as an alias.'
  errors:
  - code: NO_API_KEY
    status: 401
  - code: INVALID_API_KEY
    status: 401
  - code: API_KEY_AUTH_UNAVAILABLE
    status: 503
  in: header
  intended_use: unattended server workloads -- scheduled jobs, ETL, Databricks, agents with no person present at run time
  key_prefix: clai_live_
  key_prefix_source: published curl examples at https://closedloop.sh/docs/api-reference/introduction
  lifecycle:
    creation: Settings → API Keys in the app
    display: shown once at creation only
    revocation: immediate -- anything using a revoked key receives 401 at once
    rotation_guidance: rotate periodically, especially after team-member departures
    rotation_hazard: Incremental /insights cursors are bound to the exact key that created them. Rotating a key mid-export invalidates the cursor; restart from the last committed sync_until with the new key.
    storage: hashed with SHA-256 before storage; not retrievable by the provider afterwards
  name: ApiKeyAuth
  parameter: X-API-Key
  prohibited_use: client-side code, mobile apps, public repositories
  region_bound: true
  region_detail: Each team lives in exactly one region and each key is scoped to it. An EU key only works against https://eu.api.closedloop.sh/v1; a US key only against https://api.closedloop.sh/v1. There is no cross-region routing and no fallback.
  scope: team
  sources:
  - openapi/closedloop-public-api-openapi.yaml
  - https://closedloop.sh/docs/account/api-keys
  type: apiKey
- challenge:
    rfc9728: true
    status: 401
    www_authenticate: Bearer resource_metadata="https://mcp.closedloop.sh/.well-known/oauth-protected-resource"
  client_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  dcr_detail: The provider states clients need not pre-register -- "the OAuth Client ID and Secret are optional, and ClosedLoop AI registers your client automatically."
  declared_in_openapi: false
  discovered_by: probe
  dynamic_client_registration: true
  endpoints:
    authorization: https://mcp.closedloop.sh/authorize
    registration: https://mcp.closedloop.sh/register
    token: https://mcp.closedloop.sh/token
  flows:
  - authorization_code
  - refresh_token
  - client_credentials
  hard_separation: REST API keys DO NOT work with MCP. The provider states this explicitly on the API Keys page. An MCP caller must create an OAuth service client.
  issuer: https://mcp.closedloop.sh
  m2m:
    docs: https://closedloop.sh/docs/account/mcp-service-clients
    methods:
    - private_key_jwt with a registered RSA or P-256 public key (preferred)
    - shared secret, for clients such as LiteLLM that cannot do private_key_jwt
  name: MCPOAuth
  pkce:
  - S256
  regional_variants:
  - host: eu.mcp.closedloop.sh
    issuer: https://eu.mcp.closedloop.sh
  - difference: does NOT advertise private_key_jwt -- only none, client_secret_basic, client_secret_post
    documented: false
    host: api.closedloop.sh
    issuer: https://api.closedloop.sh/mcp
  scopes:
  - description: Invoke MCP tools. Scope name published in the authorization-server and protected-resource metadata; no per-scope description is published by the provider.
    name: mcp:tools
  - description: Read access over the MCP surface. Scope name published in the metadata; no per-scope description is published by the provider.
    name: mcp:read
  signing_algs:
  - RS256
  - ES256
  sources:
  - well-known/closedloop-mcp-oauth-authorization-server.json
  - well-known/closedloop-mcp-oauth-protected-resource.json
  - https://closedloop.sh/docs/mcp-server/overview
  - https://closedloop.sh/docs/account/mcp-service-clients
  surface: MCP
  type: oauth2
- algorithm: HMAC-SHA256 over the unmodified raw request body
  credential_location: Settings → API Keys page (same page, different credential)
  credential_name: Webhook Key
  declared_in_openapi: false
  encodings:
  - hex
  - base64
  explicit_negative: An x-api-key header does NOT authenticate an inbound webhook. Only the signing secret and the configuration confirmed at provisioning are accepted.
  headers:
  - x-webhook-signature
  - x-hub-signature-256
  - x-signature
  - typeform-signature
  name: WebhookSigningSecret
  prefix_accepted: sha256=
  rotation: self-service regenerate; no dual-secret overlap window -- previously-signed requests fail immediately
  sources:
  - https://closedloop.sh/docs/integrations/webhooks
  - https://closedloop.sh/docs/account/api-keys
  surface: inbound webhook ingestion
  type: hmac
slug: closedloop-authentication
source_filename: closedloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://closedloop.sh/docs/account/api-keys,\n  https://closedloop.sh/docs/api-reference/conventions,\n  https://closedloop.sh/docs/account/mcp-service-clients, and live OAuth metadata probes;\n  baseline derived from openapi/closedloop-public-api-openapi.yaml\ndocs: https://closedloop.sh/docs/account/api-keys\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    ClosedLoop AI runs THREE separate credential systems that are deliberately not interchangeable.\n    The published OpenAPI declares only the first of them, which is why a spec-only derivation\n    understates this provider's auth posture.\ncredential_systems:\n- id: rest-api-key\n  surface: /v1 REST API\n  scheme: ApiKeyAuth\n  declared_in_openapi: true\n- id: mcp-oauth\n  surface: MCP servers (mcp.closedloop.sh, eu.mcp.closedloop.sh, api.closedloop.sh/mcp)\n  declared_in_openapi: false\n- id: webhook-signing-secret\n  surface: inbound\
  \ webhook ingestion\n  declared_in_openapi: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  alias_parameter: apikey\n  description: |-\n    Team-scoped API key created in the app (Settings → API Keys).\n    Sent as `X-API-Key: <key>` on every request. The header name `apikey`\n    is also accepted as an alias.\n  key_prefix: clai_live_\n  key_prefix_source: published curl examples at\n    https://closedloop.sh/docs/api-reference/introduction\n  scope: team\n  region_bound: true\n  region_detail: >-\n    Each team lives in exactly one region and each key is scoped to it. An EU key only works against\n    https://eu.api.closedloop.sh/v1; a US key only against https://api.closedloop.sh/v1. There is no\n    cross-region routing and no fallback.\n  lifecycle:\n    creation: Settings → API Keys in the app\n    display: shown once at creation only\n    storage: hashed with SHA-256 before storage; not retrievable by the provider afterwards\n    revocation:\
  \ immediate -- anything using a revoked key receives 401 at once\n    rotation_guidance: rotate periodically, especially after team-member departures\n    rotation_hazard: >-\n      Incremental /insights cursors are bound to the exact key that created them. Rotating a key\n      mid-export invalidates the cursor; restart from the last committed sync_until with the new key.\n  intended_use: unattended server workloads -- scheduled jobs, ETL, Databricks, agents with no\n    person present at run time\n  prohibited_use: client-side code, mobile apps, public repositories\n  errors:\n  - status: 401\n    code: NO_API_KEY\n  - status: 401\n    code: INVALID_API_KEY\n  - status: 503\n    code: API_KEY_AUTH_UNAVAILABLE\n  sources:\n  - openapi/closedloop-public-api-openapi.yaml\n  - https://closedloop.sh/docs/account/api-keys\n- name: MCPOAuth\n  type: oauth2\n  declared_in_openapi: false\n  discovered_by: probe\n  surface: MCP\n  endpoints:\n    authorization: https://mcp.closedloop.sh/authorize\n\
  \    token: https://mcp.closedloop.sh/token\n    registration: https://mcp.closedloop.sh/register\n  issuer: https://mcp.closedloop.sh\n  flows:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  pkce: [S256]\n  client_auth_methods: [none, client_secret_basic, client_secret_post, private_key_jwt]\n  signing_algs: [RS256, ES256]\n  scopes:\n  - name: mcp:tools\n    description: Invoke MCP tools. Scope name published in the authorization-server and\n      protected-resource metadata; no per-scope description is published by the provider.\n  - name: mcp:read\n    description: Read access over the MCP surface. Scope name published in the metadata; no\n      per-scope description is published by the provider.\n  dynamic_client_registration: true\n  dcr_detail: >-\n    The provider states clients need not pre-register -- \"the OAuth Client ID and Secret are\n    optional, and ClosedLoop AI registers your client automatically.\"\n  m2m:\n    docs: https://closedloop.sh/docs/account/mcp-service-clients\n\
  \    methods:\n    - private_key_jwt with a registered RSA or P-256 public key (preferred)\n    - shared secret, for clients such as LiteLLM that cannot do private_key_jwt\n  challenge:\n    status: 401\n    www_authenticate: Bearer resource_metadata=\"https://mcp.closedloop.sh/.well-known/oauth-protected-resource\"\n    rfc9728: true\n  regional_variants:\n  - host: eu.mcp.closedloop.sh\n    issuer: https://eu.mcp.closedloop.sh\n  - host: api.closedloop.sh\n    issuer: https://api.closedloop.sh/mcp\n    documented: false\n    difference: does NOT advertise private_key_jwt -- only none, client_secret_basic,\n      client_secret_post\n  hard_separation: >-\n    REST API keys DO NOT work with MCP. The provider states this explicitly on the API Keys page.\n    An MCP caller must create an OAuth service client.\n  sources:\n  - well-known/closedloop-mcp-oauth-authorization-server.json\n  - well-known/closedloop-mcp-oauth-protected-resource.json\n  - https://closedloop.sh/docs/mcp-server/overview\n\
  \  - https://closedloop.sh/docs/account/mcp-service-clients\n- name: WebhookSigningSecret\n  type: hmac\n  declared_in_openapi: false\n  surface: inbound webhook ingestion\n  algorithm: HMAC-SHA256 over the unmodified raw request body\n  headers: [x-webhook-signature, x-hub-signature-256, x-signature, typeform-signature]\n  encodings: [hex, base64]\n  prefix_accepted: 'sha256='\n  credential_name: Webhook Key\n  credential_location: Settings → API Keys page (same page, different credential)\n  explicit_negative: >-\n    An x-api-key header does NOT authenticate an inbound webhook. Only the signing secret and the\n    configuration confirmed at provisioning are accepted.\n  rotation: self-service regenerate; no dual-secret overlap window -- previously-signed requests\n    fail immediately\n  sources:\n  - https://closedloop.sh/docs/integrations/webhooks\n  - https://closedloop.sh/docs/account/api-keys\nworkforce_sso:\n  note: >-\n    Not an API credential -- this authenticates HUMANS into\
  \ the app, and is Enterprise-plan gated.\n    Recorded because it is part of the provider's overall authentication posture and because the\n    SCIM surface it drives is a live, probeable API.\n  protocols:\n  - name: OIDC\n    idp: Okta\n    role: relying-party\n    validates: [issuer, audience, signature, state, nonce, email claim]\n    jit_provisioning: supported when enabled\n    callback: https://api.closedloop.sh/api/okta/oidc/callback\n  - name: SAML 2.0\n    idps: [Google Workspace, Microsoft Entra ID]\n    role: service-provider\n    jit_provisioning: supported\n  - name: SCIM 2.0\n    idps: [Okta, Microsoft Entra ID]\n    role: service-provider\n    base_url_template: 'https://api.closedloop.sh/api/scim/v2/{team_id}'\n    scopes: [scim.read, scim.write, entitlements.read]\n    token_model: OAuth 2.0 scoped bearer token\n    resources: [Users, Groups, Roles]\n    password_sync: not accepted -- must be left disabled\n    probe:\n      url: https://api.closedloop.sh/api/scim/v2/test/ServiceProviderConfig\n\
  \      status: 401\n      body: '{\"schemas\":[\"urn:ietf:params:scim:api:messages:2.0:Error\"],\"status\":\"401\",\"detail\":\"Bearer\n        token is required\"}'\n  - name: Global Token Revocation\n    idp: Okta (Universal Logout)\n    endpoint: https://api.closedloop.sh/api/okta/universal-logout\n    not_supported: OIDC Post Logout / browser Single Logout -- the provider says to leave the Post\n      Logout URI blank\nmtls: false\nopenid_connect_provider: false\nopenid_connect_provider_note: >-\n  No host serves /.well-known/openid-configuration -- probed on closedloop.sh, api.closedloop.sh,\n  mcp.closedloop.sh, docs.closedloop.sh, eu.api.closedloop.sh and eu.mcp.closedloop.sh, all 404.\n  ClosedLoop AI consumes OIDC as a relying party; it does not issue it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/authentication/closedloop-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Product Intelligence
- Customer Feedback
- Voice of Customer
- Product Management
- Agentic AI
- MCP
- SaaS analytics
- A2A
- SCIM
- Product Discovery
---
