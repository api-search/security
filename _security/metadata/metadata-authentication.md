---
api_key_in: []
api_specs:
- filename: metadata-mcp-server-openapi.json
  format: json
  label: Metadata MCP Server (MetadataONE)
  slug: metadata-mcp-server-metadataone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metadata/refs/heads/main/openapi/metadata-mcp-server-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Metadata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metadata declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Metadata
provider_slug: metadata
scheme_count: 2
schemes:
- display_policy: shown exactly once
  env_var: METADATA_API_KEY
  id: api_key_bearer
  in: header
  key_prefix: md1_live_
  minted_at: Settings > API Keys > Create Key
  name: Authorization
  scheme: bearer
  scoped_to: a single Metadata account
  source: https://metadata.io/developers/authentication.html
  storage: server-side only
  type: http
- authorization_endpoint: https://mcp-server.metadata.io/authorize
  client_id_metadata_document_supported: true
  dynamic_client_registration: true
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  id: oauth2
  issuer: https://mcp-server.metadata.io/
  method: probed
  note: RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata are both served anonymously. The OAuth scopes_supported (openid, offline_access) are the transport-level scopes and are DISTINCT from the seven product permission scopes documented for API keys — see scopes/metadata-scopes.yml.
  pkce:
  - S256
  registration_endpoint: https://mcp-server.metadata.io/register
  revocation_endpoint: https://mcp-server.metadata.io/revoke
  scopes_supported:
  - openid
  - offline_access
  source: https://mcp-server.metadata.io/.well-known/oauth-authorization-server
  token_endpoint: https://mcp-server.metadata.io/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: oauth2
slug: metadata-authentication
source_filename: metadata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://metadata.io/developers/authentication.html\ndocs: https://metadata.io/developers/authentication.html\nsummary: All Metadata MCP requests are authenticated with a bearer API key scoped to a single account.\n  Keys are minted in the app, stored server-side only, shown exactly once, and can be rotated or revoked.\n  The MCP endpoint additionally advertises full OAuth 2.0 authorization-server and protected-resource\n  metadata for clients that negotiate rather than carry a static key.\nschemes:\n- id: api_key_bearer\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  key_prefix: md1_live_\n  env_var: METADATA_API_KEY\n  minted_at: Settings > API Keys > Create Key\n  display_policy: shown exactly once\n  storage: server-side only\n  scoped_to: a single Metadata account\n  source: https://metadata.io/developers/authentication.html\n- id: oauth2\n  type: oauth2\n  flow: authorization_code\n  pkce:\n  -\
  \ S256\n  issuer: https://mcp-server.metadata.io/\n  authorization_endpoint: https://mcp-server.metadata.io/authorize\n  token_endpoint: https://mcp-server.metadata.io/token\n  registration_endpoint: https://mcp-server.metadata.io/register\n  revocation_endpoint: https://mcp-server.metadata.io/revoke\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - none\n  scopes_supported:\n  - openid\n  - offline_access\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  method: probed\n  source: https://mcp-server.metadata.io/.well-known/oauth-authorization-server\n  note: RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata are both served\n    anonymously. The OAuth scopes_supported (openid, offline_access) are the transport-level scopes and\n    are DISTINCT from the seven product permission scopes documented for API keys\
  \ — see scopes/metadata-scopes.yml.\nheaders:\n- name: Authorization\n  value: Bearer <METADATA_API_KEY>\n  required: true\n- name: X-Account-ID\n  required: conditional\n  note: Required on every call for users with access to multiple Metadata accounts (agencies, holding\n    companies). Call list_user_accounts first to enumerate them.\nrotation:\n  cadence_recommended: quarterly\n  triggers:\n  - employee or contractor offboarding\n  - suspected key leak (logs, shared screen, repo commit)\n  - scope expansion or reduction for the agent\n  atomic: true\n  grace_window: the old key stays valid for 15 minutes after a new one is issued; older keys are hard-revoked\n    after the grace window\n  self_service: true\n  note: Docs state to rotate rather than contact support when a key is lost.\nguidance:\n- treat tokens like passwords\n- never commit to git\n- never log them\n- never paste into chat\n- name each key after the agent that will use it (claude-code-gil, hermes-prod, paperclip-sandbox)\n\
  - scope keys to limit blast radius — an analytics-only key should not carry launch permissions\ninconsistency_note: The quickstart says to mint keys at app.metadataone.com; the authentication page says\n  platform.metadata.io. Both hosts are live and both are linked from the metadata.io nav (\"AI agency\"\n  and \"Classic view\" respectively). Recorded as published; not reconciled by API Evangelist.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metadata/refs/heads/main/authentication/metadata-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Marketing
- Marketing Automation
- Demand Generation
- Advertising
- B2B
- Artificial Intelligence
- MCP
- AI Agents
- Paid Media
- Account Based Marketing
---
