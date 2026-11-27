---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for AgentCDN
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AgentCDN Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentCDN declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentCDN
provider_slug: agentcdn-com
scheme_count: 1
schemes:
- evidence: 'Send the key as a bearer token:'
  header: Authorization
  how_to_obtain: Open Settings → API and MCP in the AgentCDN app, create an API key on the API keys card, then copy the full key.
  location: header
  name: Account API key
  scopes:
  - account:read
  - account:write
  type: http-bearer
slug: agentcdn-com-authentication
source_filename: agentcdn-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agentcdn.com/api-keys.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agentcdn.com/api-keys.md\nsources:\n- https://docs.agentcdn.com/api-keys.md\n- https://docs.agentcdn.com/quickstart.md\ndescription: Authentication schemes for AgentCDN\nschemes:\n- type: http-bearer\n  name: Account API key\n  evidence: 'Send the key as a bearer token:'\n  location: header\n  header: Authorization\n  scopes:\n  - account:read\n  - account:write\n  how_to_obtain: Open Settings → API and MCP in the AgentCDN app, create an API key on the API keys card, then copy the full key.\ndocs: https://docs.agentcdn.com/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/agentcdn-com/authentication/agentcdn-com-authentication.yml
summary_line: 1 scheme
tags:
- Video
- Artificial Intelligence
- Platform
- Media
- Integration
- Company
---
