---
api_key_in:
- header
api_specs:
- filename: fireflies-ai-apps-api-openapi.yml
  format: yaml
  label: Fireflies.ai AI Apps API
  slug: fireflies-ai-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-ai-apps-api-openapi.yml
- filename: fireflies-audio-upload-api-openapi.yml
  format: yaml
  label: Fireflies.ai Audio Upload API
  slug: fireflies-audio-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-audio-upload-api-openapi.yml
- filename: fireflies-bites-api-openapi.yml
  format: yaml
  label: Fireflies.ai Bites API
  slug: fireflies-bites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-bites-api-openapi.yml
- filename: fireflies-live-meetings-api-openapi.yml
  format: yaml
  label: Fireflies.ai Live Meetings API
  slug: fireflies-live-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-live-meetings-api-openapi.yml
- filename: fireflies-transcripts-api-openapi.yml
  format: yaml
  label: Fireflies.ai Transcripts API
  slug: fireflies-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-transcripts-api-openapi.yml
- filename: fireflies-users-api-openapi.yml
  format: yaml
  label: Fireflies.ai Users API
  slug: fireflies-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-users-api-openapi.yml
auth_types:
- http
- oauth2
description: Fireflies runs TWO distinct authentication models on the same product, and conflating them is the common integration mistake. The GraphQL API is a long-lived bearer API key with no OAuth and no scopes. The hosted MCP server is a full OAuth 2.0 authorization server with PKCE, dynamic client registration and revocation — but only two identity scopes. Upgraded from the previous derived profile, which saw only the OpenAPI BearerAuth scheme.
kind: authentication
layout: security
method: searched
name: Fireflies Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fireflies.ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fireflies.ai
provider_slug: fireflies
scheme_count: 2
schemes:
- applies_to:
  - https://api.fireflies.ai/graphql
  - wss://api.fireflies.ai (path /ws/realtime, passed as the Socket.IO auth.token parameter)
  - https://api.fireflies.ai/mcp (alternative to OAuth, via npx mcp-remote --header)
  failure:
    code: auth_failed
    http_status: 500
    note: 'Observed live: POSTing to https://api.fireflies.ai/graphql with no Authorization header returns HTTP 500 carrying code auth_failed, not a 401. Do not branch on the transport status.'
  format: Bearer <api_key>
  header: Authorization
  issuance:
    steps:
    - Log in at https://app.fireflies.ai
    - Navigate to Integrations
    - Open Fireflies API
    - Copy and store the API key securely
    url: https://app.fireflies.ai/integrations/custom/fireflies
  key_format: Not documented — no published prefix or length.
  name: BearerAuth
  rotation: Not documented. No published expiry, no programmatic rotation or revocation endpoint for API keys.
  scheme: bearer
  sources:
  - https://docs.fireflies.ai/fundamentals/authorization
  - openapi/fireflies-transcripts-api-openapi.yml
  type: http
- applies_to:
  - https://api.fireflies.ai/mcp
  - https://mcp.fireflies.ai/mcp
  discovery:
    authorization_server_metadata: /.well-known/oauth-authorization-server
    protected_resource_metadata: /.well-known/oauth-protected-resource
    specs:
    - RFC 8414
    - RFC 9728
  failure:
    code: invalid_token
    http_status: 401
    note: 'Observed live: POST tools/list with no Authorization header returns 401 invalid_token / Missing Authorization header.'
  flows:
  - authorizationUrl: https://api.fireflies.ai/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    registrationUrl: https://api.fireflies.ai/register
    revocationUrl: https://api.fireflies.ai/revoke
    scopes:
      email: Fireflies account email address
      profile: Basic Fireflies user profile
    tokenUrl: https://api.fireflies.ai/token
    token_endpoint_auth_methods:
    - client_secret_post
    - none
  name: FirefliesMCPOAuth
  sources:
  - well-known/fireflies-api-oauth-authorization-server.json
  - well-known/fireflies-mcp-oauth-authorization-server.json
  type: oauth2
slug: fireflies-authentication
source_filename: fireflies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.fireflies.ai/fundamentals/authorization\ndocs:\n- https://docs.fireflies.ai/fundamentals/authorization\n- https://docs.fireflies.ai/getting-started/mcp-configuration\ndescription: >-\n  Fireflies runs TWO distinct authentication models on the same product, and conflating them is\n  the common integration mistake. The GraphQL API is a long-lived bearer API key with no OAuth and\n  no scopes. The hosted MCP server is a full OAuth 2.0 authorization server with PKCE, dynamic\n  client registration and revocation — but only two identity scopes. Upgraded from the previous\n  derived profile, which saw only the OpenAPI BearerAuth scheme.\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  oauth2_scope_count: 2\n  mfa_or_sso: 'SSO + SCIM on the Enterprise plan (product-level, not API-level)'\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  applies_to:\n  -\
  \ https://api.fireflies.ai/graphql\n  - 'wss://api.fireflies.ai (path /ws/realtime, passed as the Socket.IO auth.token parameter)'\n  - 'https://api.fireflies.ai/mcp (alternative to OAuth, via npx mcp-remote --header)'\n  header: Authorization\n  format: 'Bearer <api_key>'\n  issuance:\n    url: https://app.fireflies.ai/integrations/custom/fireflies\n    steps:\n    - Log in at https://app.fireflies.ai\n    - Navigate to Integrations\n    - Open Fireflies API\n    - Copy and store the API key securely\n  rotation: 'Not documented. No published expiry, no programmatic rotation or revocation endpoint for API keys.'\n  key_format: 'Not documented — no published prefix or length.'\n  failure:\n    code: auth_failed\n    http_status: 500\n    note: >-\n      Observed live: POSTing to https://api.fireflies.ai/graphql with no Authorization header\n      returns HTTP 500 carrying code auth_failed, not a 401. Do not branch on the transport status.\n  sources:\n  - https://docs.fireflies.ai/fundamentals/authorization\n\
  \  - openapi/fireflies-transcripts-api-openapi.yml\n- name: FirefliesMCPOAuth\n  type: oauth2\n  applies_to:\n  - https://api.fireflies.ai/mcp\n  - https://mcp.fireflies.ai/mcp\n  discovery:\n    authorization_server_metadata: /.well-known/oauth-authorization-server\n    protected_resource_metadata: /.well-known/oauth-protected-resource\n    specs: [RFC 8414, RFC 9728]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.fireflies.ai/authorize\n    tokenUrl: https://api.fireflies.ai/token\n    revocationUrl: https://api.fireflies.ai/revoke\n    registrationUrl: https://api.fireflies.ai/register\n    grant_types: [authorization_code, refresh_token]\n    pkce: [S256]\n    token_endpoint_auth_methods: [client_secret_post, none]\n    dynamic_client_registration: true\n    scopes:\n      profile: Basic Fireflies user profile\n      email: Fireflies account email address\n  failure:\n    code: invalid_token\n    http_status: 401\n    note: 'Observed live: POST tools/list\
  \ with no Authorization header returns 401 invalid_token / Missing Authorization header.'\n  sources:\n  - well-known/fireflies-api-oauth-authorization-server.json\n  - well-known/fireflies-mcp-oauth-authorization-server.json\nauthorization_model:\n  note: >-\n    Authorization is NOT expressed in the token. The two OAuth scopes are identity scopes only —\n    there is no read/write split and no per-resource scope. What a caller may do is decided\n    downstream by (a) plan tier and (b) meeting ownership or team-admin role.\n  tier_gates:\n  - {capability: 'uploadAudio', requires: 'Pro or higher', error: paid_required}\n  - {capability: 'AskFred / AI operations', requires: 'sufficient AI credits', error: require_ai_credits}\n  - {capability: 'rule_executions_by_meeting', requires: Enterprise, error: forbidden}\n  - {capability: 'auditEvents', requires: Enterprise, error: forbidden}\n  - {capability: 'team-wide webhooks', requires: 'Enterprise + Super Admin role'}\n  role_gates:\n  - {capability:\
  \ 'shareMeeting, revokeSharedMeetingAccess, updateMeetingTitle, updateMeetingChannel, updateMeetingPrivacy', requires: 'meeting owner or team admin', error: forbidden}\n  - {capability: 'setUserRole, team-level analytics', requires: admin, error: require_elevated_privilege}\n  - {capability: 'querying users outside your team', requires: same team, error: not_in_team}\n  super_admin:\n    docs: https://docs.fireflies.ai/fundamentals/super-admin\n    note: Enterprise role granting full workspace meeting access and team-wide webhooks.\nsecurity_practices:\n  documented:\n  - Treat the API key like a password; never expose it in client-side code\n  - Store in environment variables or secure storage\n  cross_ref: security/fireflies-domain-security.yml\nx-evidence:\n  fetched: '2026-08-14'\n  probes:\n  - {url: 'https://docs.fireflies.ai/fundamentals/authorization.md', http_status: 200}\n  - {url: 'https://api.fireflies.ai/graphql', http_status: 500, body: auth_failed}\n  - {url: 'https://api.fireflies.ai/mcp',\
  \ http_status: 401, body: invalid_token}\n  - {url: 'https://api.fireflies.ai/.well-known/oauth-authorization-server', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/authentication/fireflies-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Meeting Assistant
- Transcription
- Summary
- Action Items
- GraphQL
- Meetings
- Productivity
- Collaboration
- Conversation Intelligence
---
