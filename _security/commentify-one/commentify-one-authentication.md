---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Commentify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commentify declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Commentify
provider_slug: commentify-one
scheme_count: 1
schemes:
- applies_to: https://app.commentify.one/api/mcp
  authorization_servers:
  - https://fymunivdzahrmsjcaqym.supabase.co/auth/v1
  bearer_methods_supported:
  - header
  description: The agent authenticates with OAuth. Clients connect to the server URL, the user signs in to Commentify in a browser and approves the request. Revoke an agent at any time in Settings -> Agents.
  evidence: '{"resource":"https://app.commentify.one/api/mcp","authorization_servers":["https://fymunivdzahrmsjcaqym.supabase.co/auth/v1"],"bearer_methods_supported":["header"]}'
  name: oauth2
  protected_resource_metadata: https://app.commentify.one/.well-known/oauth-protected-resource
  type: oauth2
  unauthenticated_behavior: an anonymous tools/list returns 401 (pre-flight contract discovery)
slug: commentify-one-authentication
source_filename: commentify-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Commentify authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://app.commentify.one/docs/agents\ndocs: https://app.commentify.one/docs/agents\nnote: No OpenAPI is published; the profile is read from the agents docs and the MCP server's OAuth protected-resource metadata (GET https://app.commentify.one/.well-known/oauth-protected-resource, HTTP 200). Commentify issues no API keys - the docs state that Grok Bot and the xAI API \"take only a fixed key, which Commentify does not issue.\"\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://app.commentify.one/api/mcp\n  description: The agent authenticates with OAuth. Clients connect to the server URL, the user signs in to Commentify in a browser and approves the request. Revoke an agent at any time in Settings -> Agents.\n  bearer_methods_supported:\n  - header\n  authorization_servers:\n  - https://fymunivdzahrmsjcaqym.supabase.co/auth/v1\n  protected_resource_metadata: https://app.commentify.one/.well-known/oauth-protected-resource\n\
  \  evidence: '{\"resource\":\"https://app.commentify.one/api/mcp\",\"authorization_servers\":[\"https://fymunivdzahrmsjcaqym.supabase.co/auth/v1\"],\"bearer_methods_supported\":[\"header\"]}'\n  unauthenticated_behavior: an anonymous tools/list returns 401 (pre-flight contract discovery)\n"
source_yaml_url: https://artifacts.apis.io/commentify-one/authentication/commentify-one-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Feedback
- Design Collaboration
- Comments
- MCP
- AI Agents
- Figma
- Jira
- Notion
---
