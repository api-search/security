---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chatley-ai-openapi-generated.yml
  format: yaml
  label: Chatley Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatley-ai/openapi/_ae-authored/chatley-ai-openapi-generated.yml
auth_types:
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chatley AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chatley AI secures its APIs with http-bearer and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chatley AI
provider_slug: chatley-ai
scheme_count: 2
schemes:
- applies_to: Chatley Developer API (https://api.chatley.ai)
  description: Every Developer API request is authenticated with a Chatley API key sent as a Bearer token. There are no unauthenticated endpoints. Keys are created in Integrations & API Keys -> API Keys by an account owner or administrator, are shown once, and carry the full permissions of the owning account. A key is created for one HTTP method; both Developer API endpoints are POST, so a key of any other type is rejected with METHOD_NOT_ALLOWED_FOR_KEY. Keys can carry an expiry date (API_KEY_EXPIRED) and record when they were last used.
  header: 'Authorization: Bearer chatley_your_key'
  key_prefix: chatley_
  name: bearer
  rotation: Create the replacement key first, deploy it, then deactivate the old one; a deactivated key fails immediately with API_KEY_NOT_FOUND.
  scheme: bearer
  sources:
  - https://docs.chatley.ai/api/authentication
  - openapi/_ae-authored/chatley-ai-openapi-generated.yml
  type: http
- applies_to: Chatley MCP Server (https://mcp.chatley.ai/mcp)
  authorization_servers:
  - https://mcp.chatley.ai
  description: MCP clients connect with a browser sign-in; the client registers itself automatically and the user approves it on a screen that names the client and the Chatley account. Connections can be revoked from Integrations & API Keys. The protected-resource metadata names authorization server https://mcp.chatley.ai, bearer_methods_supported [header] and scopes_supported [openid, offline_access].
  name: mcp-oauth
  scopes_supported:
  - openid
  - offline_access
  sources:
  - https://docs.chatley.ai/mcp/connecting
  - https://mcp.chatley.ai/.well-known/oauth-protected-resource
  type: oauth2
slug: chatley-ai-authentication
source_filename: chatley-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://docs.chatley.ai/api/authentication\ndocs: https://docs.chatley.ai/api/authentication\nsummary:\n  types: [http-bearer, oauth2]\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  applies_to: Chatley Developer API (https://api.chatley.ai)\n  key_prefix: chatley_\n  header: 'Authorization: Bearer chatley_your_key'\n  description: Every Developer API request is authenticated with a Chatley API key sent as a Bearer token. There are no\n    unauthenticated endpoints. Keys are created in Integrations & API Keys -> API Keys by an account owner or administrator,\n    are shown once, and carry the full permissions of the owning account. A key is created for one HTTP method; both Developer\n    API endpoints are POST, so a key of any other type is rejected with METHOD_NOT_ALLOWED_FOR_KEY. Keys can carry an expiry\n    date (API_KEY_EXPIRED) and record when they were last used.\n  rotation: Create the replacement key\
  \ first, deploy it, then deactivate the old one; a deactivated key fails immediately\n    with API_KEY_NOT_FOUND.\n  sources: [https://docs.chatley.ai/api/authentication, openapi/_ae-authored/chatley-ai-openapi-generated.yml]\n- name: mcp-oauth\n  type: oauth2\n  applies_to: Chatley MCP Server (https://mcp.chatley.ai/mcp)\n  description: MCP clients connect with a browser sign-in; the client registers itself automatically and the user approves\n    it on a screen that names the client and the Chatley account. Connections can be revoked from Integrations & API Keys.\n    The protected-resource metadata names authorization server https://mcp.chatley.ai, bearer_methods_supported [header]\n    and scopes_supported [openid, offline_access].\n  authorization_servers: [https://mcp.chatley.ai]\n  scopes_supported: [openid, offline_access]\n  sources: [https://docs.chatley.ai/mcp/connecting, https://mcp.chatley.ai/.well-known/oauth-protected-resource]\n"
source_yaml_url: https://artifacts.apis.io/chatley-ai/authentication/chatley-ai-authentication.yml
summary_line: http-bearer/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Voice Agents
- Conversational AI
- AI Receptionist
- Telephony
- SMS
- White Label
- MCP
- Lead Generation
---
