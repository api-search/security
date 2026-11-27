---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cleve-ai-folders-api-openapi.yml
  format: yaml
  label: Cleve Folders API
  slug: cleve-ai-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleve-ai/openapi/cleve-ai-folders-api-openapi.yml
- filename: cleve-ai-notes-api-openapi.yml
  format: yaml
  label: Cleve Notes API
  slug: cleve-ai-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleve-ai/openapi/cleve-ai-notes-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cleve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cleve secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cleve
provider_slug: cleve-ai
scheme_count: 2
schemes:
- description: 'Personal API key from Cleve → Settings → Developer, sent as `Authorization: Bearer <key>`.'
  key_management: In Cleve, open Settings → Developer; under REST API click Manage next to API keys, then create a key. To revoke a key, delete it from the same page.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cleve-ai-openapi.yml
  - https://docs.cleve.ai/developers/api.md
  surface: REST API (https://app.cleve.ai/api/v1)
  type: http
  workspace_binding: A personal API key acts as you, in one workspace. If you belong to several, the key works in one of them, and you can't currently choose which.
- description: The server uses OAuth 2.0. Your client opens the Cleve sign-in page, you sign in, and the client stores the access token and sends it as a Bearer token on every request. MCP doesn't use the REST API keys.
  name: mcpOAuth
  scopes_documented: false
  sources:
  - https://docs.cleve.ai/developers/mcp.md
  surface: MCP server (https://app.cleve.ai/mcp)
  type: oauth2
slug: cleve-ai-authentication
source_filename: cleve-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.cleve.ai/developers/api.md\ndocs: https://docs.cleve.ai/developers/api\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: REST API (https://app.cleve.ai/api/v1)\n  description: 'Personal API key from Cleve → Settings → Developer, sent as `Authorization: Bearer <key>`.'\n  key_management: 'In Cleve, open Settings → Developer; under REST API click Manage next to API keys, then create a key. To revoke a key, delete it from the same page.'\n  workspace_binding: 'A personal API key acts as you, in one workspace. If you belong to several, the key works in one of them, and you can''t currently choose which.'\n  sources:\n  - openapi/cleve-ai-openapi.yml\n  - https://docs.cleve.ai/developers/api.md\n- name: mcpOAuth\n  type: oauth2\n  surface: MCP server (https://app.cleve.ai/mcp)\n  description: 'The server uses OAuth 2.0. Your client opens the Cleve sign-in\
  \ page, you sign in, and the client stores the access token and sends it as a Bearer token on every request. MCP doesn''t use the REST API keys.'\n  scopes_documented: false\n  sources:\n  - https://docs.cleve.ai/developers/mcp.md\n"
source_yaml_url: https://artifacts.apis.io/cleve-ai/authentication/cleve-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Writing
- Knowledge Management
- Note Taking
- Collaboration
- MCP
- Productivity
---
