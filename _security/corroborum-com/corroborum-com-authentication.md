---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Corroborum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corroborum declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Corroborum
provider_slug: corroborum-com
scheme_count: 1
schemes:
- authorization_servers:
  - https://charming-emerald-17.authkit.app
  bearer_methods_supported:
  - header
  description: MCP OAuth sign-in. The protected-resource metadata names an authorization server at https://charming-emerald-17.authkit.app (WorkOS AuthKit); bearer token in the Authorization header.
  name: oauth2
  resource: https://mcp.corroborum.com/mcp
  scopes:
  - openid
  - profile
  - email
  - offline_access
  type: oauth2
slug: corroborum-com-authentication
source_filename: corroborum-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://mcp.corroborum.com/.well-known/oauth-protected-resource/mcp\ndocs: https://corroborum.com/docs/connect\nschemes:\n- name: oauth2\n  type: oauth2\n  description: MCP OAuth sign-in. The protected-resource metadata names an authorization server at https://charming-emerald-17.authkit.app (WorkOS AuthKit); bearer token in the Authorization header.\n  resource: https://mcp.corroborum.com/mcp\n  authorization_servers:\n  - https://charming-emerald-17.authkit.app\n  bearer_methods_supported:\n  - header\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\ndocs_statement: Your assistant sends you to our sign-in page the first time it connects. Use the same account you use on corroborum.com so your plan and allowance apply.\nnote: No API keys are documented. Read from the RFC 9728 metadata document (HTTP 200) on the documented MCP host; the authorization server itself was not called.\n"
source_yaml_url: https://artifacts.apis.io/corroborum-com/authentication/corroborum-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Academic Research
- Literature Search
- Scholarly Papers
- MCP
- AI Assistant
- Citations
---
