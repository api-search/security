---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cakewalk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cakewalk secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cakewalk
provider_slug: cakewalk
scheme_count: 3
schemes:
- applies_to: rest
  description: Public API key identifying the caller. Issued from the keys table in developer settings. Sent on every REST request.
  in: header
  name: X-API-KEY
  parameter: X-API-KEY
  sources:
  - https://www.cakewalk.security/docs/open-api-and-mcp/authentication
  type: apiKey
- applies_to: rest
  description: Secret paired with the API key, used for request integrity verification. Keys are issued with an access level of read-and-write (default) or read-only. Sent on every REST request alongside X-API-KEY.
  in: header
  name: X-API-SECRET
  parameter: X-API-SECRET
  sources:
  - https://www.cakewalk.security/docs/open-api-and-mcp/authentication
  type: apiKey
- applies_to: mcp
  description: OAuth authorization used by the hosted Cakewalk MCP server (https://mcp.getcakewalk.io/mcp). Clients register via OAuth Dynamic Client Registration and approve scopes during authorization; the granted scopes determine which MCP tools are available.
  flows:
  - flow: authorizationCode
    scopes:
    - mcp:users.read
    - mcp:workapps.read
    - mcp:requests.read
    - mcp:requests.write
  name: OAuth2
  sources:
  - https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp/connect-an-mcp-client
  type: oauth2
slug: cakewalk-authentication
source_filename: cakewalk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.cakewalk.security/docs/open-api-and-mcp/authentication\ndocs: https://www.cakewalk.security/docs/open-api-and-mcp/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The Cakewalk Open REST API authenticates with a paired API key + API secret\n    sent as HTTP headers. The hosted Cakewalk MCP server authenticates with\n    OAuth (authorization code, Dynamic Client Registration) and issues\n    scoped access tokens.\nschemes:\n- name: X-API-KEY\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: >-\n    Public API key identifying the caller. Issued from the keys table in\n    developer settings. Sent on every REST request.\n  applies_to: rest\n  sources: [https://www.cakewalk.security/docs/open-api-and-mcp/authentication]\n- name: X-API-SECRET\n  type: apiKey\n  in: header\n  parameter: X-API-SECRET\n  description: >-\n\
  \    Secret paired with the API key, used for request integrity verification.\n    Keys are issued with an access level of read-and-write (default) or\n    read-only. Sent on every REST request alongside X-API-KEY.\n  applies_to: rest\n  sources: [https://www.cakewalk.security/docs/open-api-and-mcp/authentication]\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth authorization used by the hosted Cakewalk MCP server\n    (https://mcp.getcakewalk.io/mcp). Clients register via OAuth Dynamic Client\n    Registration and approve scopes during authorization; the granted scopes\n    determine which MCP tools are available.\n  applies_to: mcp\n  flows:\n  - flow: authorizationCode\n    scopes:\n    - mcp:users.read\n    - mcp:workapps.read\n    - mcp:requests.read\n    - mcp:requests.write\n  sources: [https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp/connect-an-mcp-client]\nkey_access_levels:\n- read-and-write\n- read-only\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cakewalk/refs/heads/main/authentication/cakewalk-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Access Management
- Identity Governance
- IGA
- AI Agents
- Security
- Access Control
- MCP
- Provisioning
- SaaS Management
- Authentication
---
