---
anonymous_access: false
api_key_in: []
api_specs:
- filename: saperly-api-token-registry-api-openapi.yml
  format: yaml
  label: Saperly API Token Registry API
  slug: saperly-api-token-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-api-token-registry-api-openapi.yml
- filename: saperly-assistant-api-openapi.yml
  format: yaml
  label: Saperly Assistant API
  slug: saperly-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-assistant-api-openapi.yml
- filename: saperly-connections-api-openapi.yml
  format: yaml
  label: Saperly Connections API
  slug: saperly-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-connections-api-openapi.yml
- filename: saperly-consent-api-openapi.yml
  format: yaml
  label: Saperly Consent API
  slug: saperly-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-consent-api-openapi.yml
- filename: saperly-customvoices-api-openapi.yml
  format: yaml
  label: Saperly Custom Voices API
  slug: saperly-customvoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-customvoices-api-openapi.yml
- filename: saperly-health-api-openapi.yml
  format: yaml
  label: Saperly Health API
  slug: saperly-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-health-api-openapi.yml
- filename: saperly-keys-api-openapi.yml
  format: yaml
  label: Saperly Keys API
  slug: saperly-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-keys-api-openapi.yml
- filename: saperly-languages-api-openapi.yml
  format: yaml
  label: Saperly Languages API
  slug: saperly-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-languages-api-openapi.yml
- filename: saperly-messaging-api-openapi.yml
  format: yaml
  label: Saperly Messaging API
  slug: saperly-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-messaging-api-openapi.yml
- filename: saperly-numbers-api-openapi.yml
  format: yaml
  label: Saperly Numbers API
  slug: saperly-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-numbers-api-openapi.yml
- filename: saperly-pricing-api-openapi.yml
  format: yaml
  label: Saperly Pricing API
  slug: saperly-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-pricing-api-openapi.yml
- filename: saperly-usage-api-openapi.yml
  format: yaml
  label: Saperly Usage API
  slug: saperly-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-usage-api-openapi.yml
- filename: saperly-voice-api-openapi.yml
  format: yaml
  label: Saperly Voice API
  slug: saperly-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-voice-api-openapi.yml
- filename: saperly-voices-api-openapi.yml
  format: yaml
  label: Saperly Voices API
  slug: saperly-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-voices-api-openapi.yml
- filename: saperly-workspace-api-openapi.yml
  format: yaml
  label: Saperly Workspace API
  slug: saperly-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-workspace-api-openapi.yml
- filename: saperly-workspace-invitations-api-openapi.yml
  format: yaml
  label: Saperly Workspace Invitations API
  slug: saperly-workspace-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-workspace-invitations-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Saperly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Saperly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Saperly
provider_slug: saperly
scheme_count: 2
schemes:
- applies_to: REST API and the MCP endpoint
  description: 'One tier of scoped API key. Every request sends Authorization: Bearer sap_sk_live_…; the key carries scopes (read | write | admin), an optional number allow-list and an optional spend cap, and the workspace is always resolved from the key, never from client input. Keys are created in the dashboard (Settings → Keys) or minted as ceiling-bounded child keys by an admin-scoped key via POST /api-tokens; the plaintext token is returned once.'
  header: Authorization
  key_prefix: sap_sk_live_
  name: bearerApiKey
  scheme: bearer
  scopes:
  - read
  - write
  - admin
  type: http
- applies_to: MCP endpoint only
  authorization_url: https://saperly.com/api/auth/mcp/authorize
  description: 'MCP OAuth 2.1 for https://api.saperly.com/mcp: RFC 9728 protected-resource metadata names https://saperly.com as the authorization server; authorization code with PKCE S256, refresh tokens, dynamic client registration.'
  flow: authorizationCode
  jwks_uri: https://saperly.com/api/auth/mcp/jwks
  name: mcpOAuth
  pkce:
  - S256
  registration_url: https://saperly.com/api/auth/mcp/register
  resource: https://api.saperly.com/mcp
  scopes:
  - openid
  - profile
  - email
  - offline_access
  token_url: https://saperly.com/api/auth/mcp/token
  type: oauth2
slug: saperly-authentication
source_filename: saperly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: https://saperly.com/docs/guides/authentication; https://saperly.com/docs/api-reference; https://saperly.com/docs/sdks/mcp;\n  https://api.saperly.com/.well-known/oauth-protected-resource and https://saperly.com/.well-known/oauth-authorization-server\n  (probed 2026-10-07). The OpenAPI contract declares no securitySchemes.\ndocs: https://saperly.com/docs/guides/authentication\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  header: Authorization\n  key_prefix: sap_sk_live_\n  description: 'One tier of scoped API key. Every request sends Authorization: Bearer sap_sk_live_…; the key carries\n    scopes (read | write | admin), an optional number allow-list and an optional spend cap, and the workspace is\n    always resolved from the key, never from client input. Keys are created in the dashboard (Settings → Keys) or\n    minted as ceiling-bounded child keys by an admin-scoped key via POST /api-tokens; the plaintext\
  \ token is returned\n    once.'\n  scopes:\n  - read\n  - write\n  - admin\n  applies_to: REST API and the MCP endpoint\n- name: mcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  description: 'MCP OAuth 2.1 for https://api.saperly.com/mcp: RFC 9728 protected-resource metadata names https://saperly.com\n    as the authorization server; authorization code with PKCE S256, refresh tokens, dynamic client registration.'\n  authorization_url: https://saperly.com/api/auth/mcp/authorize\n  token_url: https://saperly.com/api/auth/mcp/token\n  registration_url: https://saperly.com/api/auth/mcp/register\n  jwks_uri: https://saperly.com/api/auth/mcp/jwks\n  pkce:\n  - S256\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  resource: https://api.saperly.com/mcp\n  applies_to: MCP endpoint only\nerrors:\n  '401': Unauthorized — no bearer token on the request\n  '403': AuthorizationDenied — unrecognized, revoked, missing scope, or number outside the allow-list\n  '402': SpendLimitExceeded\
  \ — the key's spend cap was hit at reserve time\nnotes: Human dashboard members get abilities from their org role (owner/admin vs member) rather than a key grant.\n  No OAuth is offered for the REST API itself.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/authentication/saperly-authentication.yml
summary_line: 2 schemes
tags:
- Telephony
- Voice
- SMS
- Phone Numbers
- AI Agents
- Consent
- Compliance
- MCP
- Messaging
- Communications
---
