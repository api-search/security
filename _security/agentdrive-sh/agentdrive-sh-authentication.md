---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentdrive-sh-openapi-generated.yml
  format: yaml
  label: AgentDrive API
  slug: agentdrive-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdrive-sh/openapi/_ae-authored/agentdrive-sh-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Agentdrive Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentDrive declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: AgentDrive
provider_slug: agentdrive-sh
scheme_count: 5
schemes:
- description: 'Bearer API key authentication. Use Authorization: Bearer <api_key>'
  flows: {}
  type: oauth2
- description: 'Share token authentication. Use Authorization: Bearer <share_token>'
  flows: {}
  type: oauth2
- description: 'Magic‑link session authentication via Cookie: session=<session_id>'
  flows: {}
  type: cookie
- description: Indicates the client platform (claude-code, codex, cursor, etc.)
  name: X-Agent-Platform
  type: header
- description: Indicates the agent role (planner, coder, reviewer, etc.)
  name: X-Agent-Role
  type: header
slug: agentdrive-sh-authentication
source_filename: agentdrive-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://agentdrive.sh/docs/rest-api\nschemes:\n  - type: oauth2\n    description: \"Bearer API key authentication. Use Authorization: Bearer <api_key>\"\n    flows: {}\n  - type: oauth2\n    description: \"Share token authentication. Use Authorization: Bearer <share_token>\"\n    flows: {}\n  - type: cookie\n    description: \"Magic‑link session authentication via Cookie: session=<session_id>\"\n    flows: {}\n  - type: header\n    name: X-Agent-Platform\n    description: \"Indicates the client platform (claude-code, codex, cursor, etc.)\"\n  - type: header\n    name: X-Agent-Role\n    description: \"Indicates the agent role (planner, coder, reviewer, etc.)\"\n"
source_yaml_url: https://artifacts.apis.io/agentdrive-sh/authentication/agentdrive-sh-authentication.yml
summary_line: 5 schemes
tags:
- AgentDrive
- Artificial Intelligence
- Multi-Agent
- Workspace
- Memory
- MCP
---
