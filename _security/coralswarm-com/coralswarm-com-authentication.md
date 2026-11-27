---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CoralSwarm Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoralSwarm declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CoralSwarm
provider_slug: coralswarm-com
scheme_count: 1
schemes:
- applies_to: https://api.coralswarm.com/mcp
  description: Auth is OAuth (Clerk) with dynamic client registration — there is no API key to paste and nothing to put in a config file.
  dynamic_client_registration: true
  issuer_host: clerk.coralswarm.com
  name: Clerk OAuth
  note: The MCP endpoint answers an anonymous request with 401 and a protected-resource metadata pointer (pre-flight contract discovery, status 401). The README notes the MCP URL must match the server's protected-resource metadata. Tokens can be bound to one ocean, which limits what an agent can see (homepage FAQ).
  type: oauth2
slug: coralswarm-com-authentication
source_filename: coralswarm-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://github.com/CoralSwarm/coralswarm-connect\ndocs: https://github.com/CoralSwarm/coralswarm-connect#install\nschemes:\n- type: oauth2\n  name: Clerk OAuth\n  description: \"Auth is OAuth (Clerk) with dynamic client registration — there is no API key to paste and nothing to put in a config file.\"\n  issuer_host: clerk.coralswarm.com\n  dynamic_client_registration: true\n  applies_to: https://api.coralswarm.com/mcp\n  note: The MCP endpoint answers an anonymous request with 401 and a protected-resource metadata pointer (pre-flight contract discovery, status 401). The README notes the MCP URL must match the server's protected-resource metadata. Tokens can be bound to one ocean, which limits what an agent can see (homepage FAQ).\napi_keys: false\n"
source_yaml_url: https://artifacts.apis.io/coralswarm-com/authentication/coralswarm-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Organizational Memory
- Knowledge Management
- AI Agents
- MCP
- Search
- Productivity
- Collaboration
---
