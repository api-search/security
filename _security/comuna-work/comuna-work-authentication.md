---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Comuna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comuna declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Comuna
provider_slug: comuna-work
scheme_count: 1
schemes:
- applies_to:
  - https://api.comuna.work/mcp
  - https://api.comuna.work/api/v1/
  authorization_server: https://nujbxusvzbswqqbbsqqb.supabase.co/auth/v1
  bearer_methods_supported:
  - header
  client_registration: 'Docs: "register your client at the well-known endpoint, walk the user through approval, get a Bearer token."'
  description: OAuth2 (Supabase OAuth Server). "The first time a client connects, you go through an approval flow and authorize the client with your Comuna account. After that, the client gets a Bearer token it uses for every call."
  evidence:
  - http_status: 200
    note: RFC 9728 protected-resource metadata names the Supabase authorization server, header bearer method and scopes.
    url: https://api.comuna.work/.well-known/oauth-protected-resource
  - quote: Authentication is OAuth2 via Supabase. After approval, Comuna issues a token that the AI client uses to call MCP tools with that user's permissions (RLS-enforced).
    url: https://comuna.work/llms-full.txt
  name: oauth2
  type: oauth2
slug: comuna-work-authentication
source_filename: comuna-work-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comuna.work/integrations/mcp/\ndocs: https://comuna.work/integrations/mcp/\nschemes:\n- name: oauth2\n  type: oauth2\n  description: 'OAuth2 (Supabase OAuth Server). \"The first time a client connects, you go through an approval flow and authorize the client with your Comuna account. After that, the client gets a Bearer token it uses for every call.\"'\n  authorization_server: https://nujbxusvzbswqqbbsqqb.supabase.co/auth/v1\n  bearer_methods_supported:\n  - header\n  client_registration: 'Docs: \"register your client at the well-known endpoint, walk the user through approval, get a Bearer token.\"'\n  applies_to:\n  - https://api.comuna.work/mcp\n  - https://api.comuna.work/api/v1/\n  evidence:\n  - url: https://api.comuna.work/.well-known/oauth-protected-resource\n    http_status: 200\n    note: RFC 9728 protected-resource metadata names the Supabase authorization server, header bearer method and scopes.\n  - url:\
  \ https://comuna.work/llms-full.txt\n    quote: 'Authentication is OAuth2 via Supabase. After approval, Comuna issues a token that the AI client uses to call MCP tools with that user''s permissions (RLS-enforced).'\napi_keys: 'None. The site states \"No API keys, no proxy: Comuna talks to your AI client.\" (https://comuna.work/llms.txt)'\nnote: No OpenAPI is held (https://api.comuna.work/openapi.yaml named by the docs returned 404 on 2026-11-04), so nothing was derived from a contract. The OAuth flow itself was not exercised.\n"
source_yaml_url: https://artifacts.apis.io/comuna-work/authentication/comuna-work-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Project Management
- Kanban
- Collaboration
- AI Agents
- MCP
- Productivity
---
