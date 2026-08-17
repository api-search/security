---
api_key_in: []
api_specs:
- filename: outreach-openapi.yml
  format: yaml
  label: Outreach REST API
  slug: outreach-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outreach/refs/heads/main/openapi/outreach-openapi.yml
- filename: outreach-webhooks-asyncapi.yml
  format: yaml
  label: Outreach Webhooks
  slug: outreach-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/outreach/refs/heads/main/webhooks/outreach-webhooks-asyncapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Outreach Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Outreach secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Outreach
provider_slug: outreach
scheme_count: 3
schemes:
- applies_to: All 253 operations (declared as the global `security` requirement in the OpenAPI)
  bearerFormat: JWT
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/_original/outreach-openapi.json
  token_source: OAuth 2.0 authorization code flow
  type: http
- applies_to: 63 of 253 operations declare `s2sAuthToken` alongside `bearerAuth`
  bearerFormat: JWT
  in: header
  name: s2sAuthToken
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/_original/outreach-openapi.json
  - https://developers.outreach.io/api/s2s-access
  token_source: Server-to-server token exchange, signed with a customer-registered RSA public key
  type: http
- applies_to: https://api.outreach.io/mcp
  dynamic_client_registration: true
  flow: authorizationCode
  name: OAuth 2.1 (MCP)
  pkce: S256
  sources:
  - https://api.outreach.io/.well-known/oauth-authorization-server
  - https://developers.outreach.io/mcp-server/authentication
  type: oauth2
slug: outreach-authentication
source_filename: outreach-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.outreach.io/api/getting-started\ndocs:\n- https://developers.outreach.io/api/getting-started\n- https://developers.outreach.io/api/oauth\n- https://developers.outreach.io/api/s2s-access\n- https://developers.outreach.io/mcp-server/authentication\nprovider: Outreach\nproviderId: outreach\nsummary:\n  types:\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  primary: OAuth 2.0 authorization code (REST) / OAuth 2.1 + PKCE + DCR (MCP)\n  api_keys_supported: false\n  note: >-\n    Derived from the OpenAPI this profile is thin — the spec declares only two HTTP bearer schemes\n    (`bearerAuth`, `s2sAuthToken`) and no oauth2 scheme at all, which understates the real model. Upgraded\n    from the provider's own auth documentation: the REST API is OAuth 2.0 authorization-code only, the MCP\n    server is OAuth 2.1 with PKCE and Dynamic Client Registration, and S2S is a separate JWT\n\
  \    application-identity token. Outreach issues no static API keys; an application must never ask a user for\n    one.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  applies_to: All 253 operations (declared as the global `security` requirement in the OpenAPI)\n  token_source: OAuth 2.0 authorization code flow\n  sources:\n  - openapi/_original/outreach-openapi.json\n- name: s2sAuthToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  applies_to: 63 of 253 operations declare `s2sAuthToken` alongside `bearerAuth`\n  token_source: Server-to-server token exchange, signed with a customer-registered RSA public key\n  sources:\n  - openapi/_original/outreach-openapi.json\n  - https://developers.outreach.io/api/s2s-access\n- name: OAuth 2.1 (MCP)\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  dynamic_client_registration: true\n  applies_to: https://api.outreach.io/mcp\n\
  \  sources:\n  - https://api.outreach.io/.well-known/oauth-authorization-server\n  - https://developers.outreach.io/mcp-server/authentication\noauth2:\n  flow: authorizationCode\n  authorization_url: https://api.outreach.io/oauth/authorize\n  token_url: https://api.outreach.io/oauth/token\n  response_type: code\n  state_parameter: supported and recommended for CSRF protection\n  refresh: grant_type=refresh_token\n  token_response_fields:\n  - access_token\n  - token_type\n  - expires_in\n  - refresh_token\n  - scope\n  - created_at\n  access_token_ttl_seconds: 7200\n  refresh_token_ttl_days: 14\n  max_active_refresh_tokens: 100\n  mint_throttle: one access token per user/application per 60 seconds; 429 beyond that\n  credential_environments:\n  - name: development\n    provisioning: immediate\n    review: none\n    limits: Usable without limitation by up to 10 users from the owning org; other users (or more than 10\n      from the owning org) must re-authorize weekly. Consent screen warns\
  \ the app is unreviewed.\n  - name: production\n    provisioning: after the publishing process and review\n    limits: none stated\n  secret_handling: OAuth client secrets are displayed once at generation and cannot be redisplayed; use\n    Regenerate to mint new ones.\n  scopes: scopes/outreach-scopes.yml\nmcp_oauth:\n  authorization_server: https://api.outreach.io\n  metadata: https://api.outreach.io/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://api.outreach.io/.well-known/oauth-protected-resource\n  authorization_endpoint: https://api.outreach.io/mcpOAuth/authorize\n  token_endpoint: https://api.outreach.io/mcpOAuth/token\n  registration_endpoint: https://api.outreach.io/mcpOAuth/register\n  registration_spec: RFC 7591 Dynamic Client Registration\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_post]\n  grant_types_supported: [authorization_code, refresh_token]\n  scopes_supported: [prospects.all]\n\
  \  challenge: 'POST to the MCP endpoint without a token returns 401 with WWW-Authenticate: Bearer\n    resource_metadata=\"https://api.outreach.io/.well-known/oauth-protected-resource\" (RFC 9728)'\n  enterprise_control: DCR means any MCP client can self-register; Outreach directs enterprises to restrict\n    which clients may connect using IDP-level group restrictions, device trust or conditional access.\ns2s:\n  purpose: Server-side access without an interactive consent flow\n  identity: application + organization, NOT a user\n  key_registration: customer uploads one or more PEM-encoded RSA public keys in the developer portal\n  key_generation: openssl genrsa -out outreach_private_key.pem 2048\n  scope_subset: true\n  limitations: Read operations work broadly; some writes require additional data (e.g. an authorizer user\n    id) and some writes are unsupported entirely because there is no user actor.\n  docs: https://developers.outreach.io/api/s2s-access\nrequest_headers:\n  authorization:\
  \ 'Bearer <access_token>'\n  content_type: application/vnd.api+json\nerror_responses:\n- status: 403\n  id: unauthorizedOauthScope\n  meaning: token lacks the required scope\n- status: 403\n  id: unauthorizedRequest\n  meaning: token has the scope but the user's governance permissions do not allow the action\n- status: 429\n  id: rateLimitExceeded\n  meaning: includes token minting more than once per 60 seconds\nsecurity_posture:\n  short_lived_tokens: 'Since 2021-01-01 all issued tokens are short-lived; tokens older than 1.5 years were\n    deleted.'\n  revocation: Revoking the customer's authorization grant invalidates tokens; for MCP, disabling the user at\n    the IDP immediately revokes access.\n  audit: MCP tool calls are attributed to the authenticated user in Outreach activity history.\n  advisory: https://developers.outreach.io/guides/warning\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outreach/refs/heads/main/authentication/outreach-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Sales
- Sales Engagement
- Sequences
- CRM
- Email
- Revenue Operations
- Sales Execution
- Prospecting
- Agents
- MCP
---
