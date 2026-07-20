---
api_key_in:
- header
api_specs:
- filename: fellow-webhooks-asyncapi.yml
  format: yaml
  label: Fellow Developer API
  slug: fellow-developer-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/asyncapi/fellow-webhooks-asyncapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fellow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fellow secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fellow
provider_slug: fellow
scheme_count: 2
schemes:
- applies_to: Fellow Developer REST API
  docs: https://developers.fellow.ai/reference/authentication-1
  in: header
  name: ApiKeyAuth
  notes: Personal API keys are generated per user under User Settings -> Developer API. Keys are shown once and stored hashed. Multiple keys per user are supported (one per application recommended for selective revocation). Keys may be issued with "privileged access" (super-admin) that widens read scope to the whole workspace; write operations always remain scoped to the key owner. The API must be enabled workspace-wide by an admin under Security settings. Missing/invalid key returns 401 Unauthorized; a valid key without resource access returns 403.
  parameter_name: X-API-KEY
  type: apiKey
- applies_to: Fellow hosted MCP server (https://fellow.app/mcp)
  flows:
  - authorizationUrl: https://fellow.app/mcp/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://fellow.app/mcp/register
    revocationUrl: https://fellow.app/mcp/revoke
    scopes:
    - read_calendar
    - read_meeting_content
    - read_action_items
    - read_channels
    - write_meeting_agenda
    tokenUrl: https://fellow.app/mcp/token
  name: MCPOAuth
  source: well-known/fellow-oauth-authorization-server.json
  type: oauth2
slug: fellow-authentication
source_filename: fellow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.fellow.ai/reference/authentication-1\ndocs: https://developers.fellow.ai/reference/authentication-1\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_name: X-API-KEY\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  applies_to: Fellow Developer REST API\n  docs: https://developers.fellow.ai/reference/authentication-1\n  notes: >-\n    Personal API keys are generated per user under User Settings -> Developer API.\n    Keys are shown once and stored hashed. Multiple keys per user are supported\n    (one per application recommended for selective revocation). Keys may be issued\n    with \"privileged access\" (super-admin) that widens read scope to the whole\n    workspace; write operations always remain scoped to the key owner. The API must\n    be enabled workspace-wide by an admin under Security settings. Missing/invalid\n\
  \    key returns 401 Unauthorized; a valid key without resource access returns 403.\n- name: MCPOAuth\n  type: oauth2\n  applies_to: Fellow hosted MCP server (https://fellow.app/mcp)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fellow.app/mcp/authorize\n    tokenUrl: https://fellow.app/mcp/token\n    registrationUrl: https://fellow.app/mcp/register\n    revocationUrl: https://fellow.app/mcp/revoke\n    pkce: S256\n    scopes:\n    - read_calendar\n    - read_meeting_content\n    - read_action_items\n    - read_channels\n    - write_meeting_agenda\n  source: well-known/fellow-oauth-authorization-server.json\naccess_model: >-\n  Both mechanisms enforce Fellow's in-app access rules: an API key or MCP token can\n  only reach resources the owner can already access in the Fellow interface\n  (attendee of the event, explicitly shared, or in a channel where the object was\n  published).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/authentication/fellow-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Saas
- Meetings
- AI
- Meeting Notes
- Transcription
- Productivity
- Action Items
- Webhooks
- MCP
---
