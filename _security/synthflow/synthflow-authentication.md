---
api_key_in:
- header
api_specs:
- filename: synthflow-default-api-openapi.yml
  format: yaml
  label: Synthflow Default API
  slug: synthflow-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-default-api-openapi.yml
- filename: synthflow-chat-api-openapi.yml
  format: yaml
  label: Synthflow Chat API
  slug: synthflow-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-chat-api-openapi.yml
- filename: synthflow-contacts-api-openapi.yml
  format: yaml
  label: Synthflow Contacts API
  slug: synthflow-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-contacts-api-openapi.yml
- filename: synthflow-mcp-api-openapi.yml
  format: yaml
  label: Synthflow MCP API
  slug: synthflow-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-mcp-api-openapi.yml
- filename: synthflow-memorystores-api-openapi.yml
  format: yaml
  label: Synthflow Memory Stores API
  slug: synthflow-memorystores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-memorystores-api-openapi.yml
- filename: synthflow-phonenumbers-api-openapi.yml
  format: yaml
  label: Synthflow Phone Numbers API
  slug: synthflow-phonenumbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-phonenumbers-api-openapi.yml
- filename: synthflow-webhooklogs-api-openapi.yml
  format: yaml
  label: Synthflow Webhook Logs API
  slug: synthflow-webhooklogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-webhooklogs-api-openapi.yml
auth_types:
- http
- oauth2
description: Synthflow runs two different authentication models on two different surfaces. The REST Platform API uses a single static workspace API key sent as an HTTP bearer token. The hosted MCP server uses OAuth 2.0, delegated to WorkOS AuthKit, with dynamic client registration and PKCE. They do not share credentials.
kind: authentication
layout: security
method: searched
name: Synthflow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
overview: Synthflow secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and refreshToken flow(s).
provider_name: Synthflow
provider_slug: synthflow
scheme_count: 3
schemes:
- applied_to: 100 of 100 operations (global security requirement)
  expiry: Not documented — keys appear to be long-lived until deleted.
  format: Bearer <SYNTHFLOW_API_KEY>
  header: Authorization
  key_management: Admin -> Workspace Settings -> API Keys
  key_prefix: none
  mfa_prerequisite: Where the workspace requires 2FA, a user must have 2FA enabled to create or view API keys.
  name: sec0
  note: A single static key carries full workspace authority across all 100 operations, including delete-assistant and voice-call (which places real, billable calls). There is no read-only key, no per-resource scoping and no key-level permission model, so an agent given a key to read call logs can also delete every agent in the workspace.
  role_gated: Key creation and viewing depend on the user role.
  rotation_guidance: Provider advises rotating keys periodically and deleting unused keys.
  scheme: bearer
  scopes: none
  scoping: workspace
  sources:
  - openapi/_original/synthflow-openapi.json
  surface: rest
  type: http
  verification: Synthflow publishes a read-only verification call — GET https://api.synthflow.ai/v2/assistants/ (list-assistant) takes no required parameters, so a 200 confirms the key.
- authorization_server: https://kind-prelude-27.authkit.app
  authorization_server_metadata: https://kind-prelude-27.authkit.app/.well-known/oauth-authorization-server
  bearer_methods_supported:
  - header
  dynamic_client_registration: https://kind-prelude-27.authkit.app/oauth2/register
  flows:
  - authorizationUrl: https://kind-prelude-27.authkit.app/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://kind-prelude-27.authkit.app/oauth2/device_authorization
    flow: deviceCode
    grant_type: urn:ietf:params:oauth:grant-type:device_code
  - flow: refreshToken
    tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token
  introspection_endpoint: https://kind-prelude-27.authkit.app/oauth2/introspection
  issuer: https://kind-prelude-27.authkit.app
  jwks_uri: https://kind-prelude-27.authkit.app/oauth2/jwks
  name: mcp-oauth
  protected_resource_metadata: https://mcp.synthflow.ai/.well-known/oauth-protected-resource
  provenance_note: kind-prelude-27.authkit.app is a WorkOS AuthKit tenant, not a synthflow.ai host. It is named as the authorization server by Synthflow's OWN protected-resource metadata served from mcp.synthflow.ai, and Synthflow's security documentation independently states that WorkOS is its identity infrastructure provider. This is a delegated IdP, not a foreign contract.
  resource: https://mcp.synthflow.ai/mcp
  response_modes_supported:
  - query
  response_types_supported:
  - code
  scopes:
  - openid
  - profile
  - email
  - offline_access
  see: scopes/synthflow-scopes.yml
  surface: mcp
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
- name: docs-mcp
  note: The Fern documentation MCP server answers initialize and tools/list anonymously.
  surface: mcp-docs
  type: none
  url: https://docs.synthflow.ai/_mcp/server
slug: synthflow-authentication
source_filename: synthflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.synthflow.ai/authentication\ndocs: https://docs.synthflow.ai/authentication\nderived_from: openapi/_original/synthflow-openapi.json\ndescription: >-\n  Synthflow runs two different authentication models on two different surfaces. The REST\n  Platform API uses a single static workspace API key sent as an HTTP bearer token. The\n  hosted MCP server uses OAuth 2.0, delegated to WorkOS AuthKit, with dynamic client\n  registration and PKCE. They do not share credentials.\n\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, deviceCode, refreshToken]\n  surfaces: 2\n\nschemes:\n  - name: sec0\n    surface: rest\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: 'Bearer <SYNTHFLOW_API_KEY>'\n    sources: [openapi/_original/synthflow-openapi.json]\n    applied_to: '100 of 100 operations (global security requirement)'\n    key_prefix: none\n    key_management:\
  \ 'Admin -> Workspace Settings -> API Keys'\n    scoping: workspace\n    role_gated: 'Key creation and viewing depend on the user role.'\n    mfa_prerequisite: 'Where the workspace requires 2FA, a user must have 2FA enabled to create or view API keys.'\n    rotation_guidance: 'Provider advises rotating keys periodically and deleting unused keys.'\n    verification: >-\n      Synthflow publishes a read-only verification call — GET\n      https://api.synthflow.ai/v2/assistants/ (list-assistant) takes no required\n      parameters, so a 200 confirms the key.\n    expiry: 'Not documented — keys appear to be long-lived until deleted.'\n    scopes: none\n    note: >-\n      A single static key carries full workspace authority across all 100 operations,\n      including delete-assistant and voice-call (which places real, billable calls). There\n      is no read-only key, no per-resource scoping and no key-level permission model, so an\n      agent given a key to read call logs can also delete\
  \ every agent in the workspace.\n  - name: mcp-oauth\n    surface: mcp\n    type: oauth2\n    resource: https://mcp.synthflow.ai/mcp\n    protected_resource_metadata: https://mcp.synthflow.ai/.well-known/oauth-protected-resource\n    authorization_server: https://kind-prelude-27.authkit.app\n    authorization_server_metadata: https://kind-prelude-27.authkit.app/.well-known/oauth-authorization-server\n    issuer: https://kind-prelude-27.authkit.app\n    bearer_methods_supported: [header]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://kind-prelude-27.authkit.app/oauth2/authorize\n        tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token\n        pkce: S256\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://kind-prelude-27.authkit.app/oauth2/device_authorization\n        grant_type: 'urn:ietf:params:oauth:grant-type:device_code'\n      - flow: refreshToken\n        tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token\n    dynamic_client_registration:\
  \ https://kind-prelude-27.authkit.app/oauth2/register\n    introspection_endpoint: https://kind-prelude-27.authkit.app/oauth2/introspection\n    jwks_uri: https://kind-prelude-27.authkit.app/oauth2/jwks\n    token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n    response_types_supported: [code]\n    response_modes_supported: [query]\n    scopes: [openid, profile, email, offline_access]\n    see: scopes/synthflow-scopes.yml\n    provenance_note: >-\n      kind-prelude-27.authkit.app is a WorkOS AuthKit tenant, not a synthflow.ai host. It\n      is named as the authorization server by Synthflow's OWN protected-resource metadata\n      served from mcp.synthflow.ai, and Synthflow's security documentation independently\n      states that WorkOS is its identity infrastructure provider. This is a delegated IdP,\n      not a foreign contract.\n  - name: docs-mcp\n    surface: mcp-docs\n    type: none\n    url: https://docs.synthflow.ai/_mcp/server\n    note:\
  \ 'The Fern documentation MCP server answers initialize and tools/list anonymously.'\n\nworkspace_authentication:\n  description: 'How humans sign in, as distinct from how API callers authenticate.'\n  docs: https://docs.synthflow.ai/security\n  methods:\n    - {method: email-password, mfa: 'TOTP 2FA with backup codes, optionally mandatory workspace-wide'}\n    - {method: google, mfa: 'TOTP 2FA'}\n    - {method: sso-saml, provider: WorkOS, plan: Enterprise, identity_providers: [Okta, Entra ID, Google SAML, Auth0]}\n  allowed_email_domains: true\n\nwebhook_authentication:\n  direction: inbound-to-customer\n  mechanism: HMAC-SHA256\n  header: HTTP_SYNTHFLOW_SIGNATURE\n  see: asyncapi/synthflow-webhooks.yml\n\ngaps:\n  - 'No scoped or read-only API keys — one key, full workspace authority.'\n  - 'No documented key expiry or automatic rotation.'\n  - 'No OAuth on the REST API, so a third-party integration must hold a customer''s raw workspace key.'\n  - 'No /.well-known/openid-configuration\
  \ on any synthflow.ai host.'\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n    - {url: 'https://docs.synthflow.ai/authentication.md', status: 200}\n    - {url: 'https://mcp.synthflow.ai/mcp', status: 401, detail: 'WWW-Authenticate: Bearer error=\"unauthorized\"'}\n    - {url: 'https://mcp.synthflow.ai/.well-known/oauth-protected-resource', status: 200}\n    - {url: 'https://kind-prelude-27.authkit.app/.well-known/oauth-authorization-server', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/authentication/synthflow-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Voice
- Voice Agents
- No-Code
- Telephony
- Phone
- Outbound
- Inbound
- CRM
- Webhook
- Custom Actions
- HIPAA
- SOC 2
- MCP
- Agent Skills
- Conversational AI
- SIP
- Simulations
- Knowledge Base
---
