---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CNAPS.AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: CNAPS.AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CNAPS.AI
provider_slug: cnaps-ai
scheme_count: 2
schemes:
- applies_to:
  - REST API batch runs
  - MCP server (n8n)
  docs: https://docs.cnaps.ai/
  header: x-api-key
  in: header
  key_lifecycle: Created in the web console with a description and an expiration; shown only once; can be deactivated, regenerated or deleted.
  name: apiKey
  type: apiKey
- applies_to:
  - MCP server (Claude
  - ChatGPT
  - Zapier
  - n8n)
  docs: https://docs.cnaps.ai/mcp-user-guide
  dynamic_client_registration: true
  name: oauth2
  pkce: S256
  protected_resource_metadata: https://mcp.cnaps.ai/.well-known/oauth-protected-resource
  revocation: Disconnecting an app under Account Settings > Security > Connected apps revokes its tokens immediately.
  scopes_ref: scopes/cnaps-ai-scopes.yml
  type: oauth2
  version: OAuth 2.1
slug: cnaps-ai-authentication
source_filename: cnaps-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.cnaps.ai/mcp-user-guide\ndocs: https://docs.cnaps.ai/mcp-user-guide\nsummary: >-\n  Two schemes. The REST API (POST https://cnaps.ai/api/v1/batch-runs/run) and the n8n MCP connection use a workspace API key sent in the\n  x-api-key header. The remote MCP server (https://mcp.cnaps.ai/mcp) also supports OAuth 2.1 with dynamic client registration and PKCE (S256),\n  advertised at /.well-known/oauth-protected-resource; Claude, ChatGPT and Zapier connect with OAuth only. API keys are created, viewed,\n  deactivated, regenerated and deleted only in the web console; key management is deliberately not exposed as an MCP tool or API endpoint.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  header: x-api-key\n  applies_to: [REST API batch runs, MCP server (n8n)]\n  key_lifecycle: Created in the web console with a description and an expiration; shown only once; can be deactivated, regenerated or deleted.\n  docs:\
  \ https://docs.cnaps.ai/\n- name: oauth2\n  type: oauth2\n  version: OAuth 2.1\n  dynamic_client_registration: true\n  pkce: S256\n  protected_resource_metadata: https://mcp.cnaps.ai/.well-known/oauth-protected-resource\n  applies_to: [MCP server (Claude, ChatGPT, Zapier, n8n)]\n  scopes_ref: scopes/cnaps-ai-scopes.yml\n  revocation: Disconnecting an app under Account Settings > Security > Connected apps revokes its tokens immediately.\n  docs: https://docs.cnaps.ai/mcp-user-guide\n"
source_yaml_url: https://artifacts.apis.io/cnaps-ai/authentication/cnaps-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Generative AI
- Workflow Automation
- No-Code
- Image Generation
- Video Generation
- MCP
---
