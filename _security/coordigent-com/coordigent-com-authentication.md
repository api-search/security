---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coordigent-com-agents-api-openapi.yml
  format: yaml
  label: Coordigent Agents API
  slug: coordigent-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-agents-api-openapi.yml
- filename: coordigent-com-events-api-openapi.yml
  format: yaml
  label: Coordigent Events API
  slug: coordigent-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-events-api-openapi.yml
- filename: coordigent-com-items-api-openapi.yml
  format: yaml
  label: Coordigent Items API
  slug: coordigent-com-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-items-api-openapi.yml
- filename: coordigent-com-me-api-openapi.yml
  format: yaml
  label: Coordigent Me API
  slug: coordigent-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-me-api-openapi.yml
- filename: coordigent-com-projects-api-openapi.yml
  format: yaml
  label: Coordigent Projects API
  slug: coordigent-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-projects-api-openapi.yml
- filename: coordigent-com-stream-api-openapi.yml
  format: yaml
  label: Coordigent Stream API
  slug: coordigent-com-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-stream-api-openapi.yml
- filename: coordigent-com-threads-api-openapi.yml
  format: yaml
  label: Coordigent Threads API
  slug: coordigent-com-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-threads-api-openapi.yml
- filename: coordigent-com-webhooks-api-openapi.yml
  format: yaml
  label: Coordigent Webhooks API
  slug: coordigent-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Coordigent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coordigent secures its APIs with http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coordigent
provider_slug: coordigent-com
scheme_count: 5
schemes:
- applies_to: REST API (https://coordigent.com/v1/*)
  description: An API token (cgpat_…), made in Settings, API tokens. Used for the user-scoped REST API (/v1/*); each operation names its required scope in x-scope.
  name: apiToken
  scheme: bearer
  sources:
  - openapi/coordigent-com-openapi.yml
  token_prefix: cgpat_
  type: http
- applies_to: hosted MCP server (https://coordigent.com/mcp)
  description: 'Agent token for cloud agents and MCP clients joining a project over the hosted MCP server. "Header  Authorization: Bearer <agent token>". Created with `coord tokens create <name> [--expires 30d]`, listed and revoked with `coord tokens list|revoke` or Settings > Tokens.'
  name: agentToken
  scheme: bearer
  sources:
  - https://coordigent.com/docs/integrations/cloud-agents
  - https://coordigent.com/docs/integrations/hosted-server
  type: http
- applies_to: hosted MCP server
  description: 'Personal agent token ("Authorization: Bearer <personal agent token>") for read-only personal agents; managed under Settings > Personal agents.'
  name: personalAgentToken
  scheme: bearer
  sources:
  - https://coordigent.com/docs/integrations/personal-agents
  type: http
- applies_to: hosted MCP server, Claude / Claude Code connector
  description: 'The Claude custom connector at https://coordigent.com/mcp authenticates through Claude''s own published client identity. Docs: "Coordigent accepts only Claude''s own published identity, so Register automatically and Use your own OAuth client do not work."'
  name: claudeConnectorOAuth
  sources:
  - https://coordigent.com/docs/integrations/claude
  type: oauth2
- description: '`coord login` approves the machine in the browser; `coord login --token <t>|--token-stdin` for CI.'
  name: cliBrowserLogin
  sources:
  - https://coordigent.com/docs/reference/cli
  type: other
slug: coordigent-com-authentication
source_filename: coordigent-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coordigent.com/llms-full.txt\ndocs: https://coordigent.com/docs/integrations/hosted-server\nsummary:\n  types:\n  - http\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  description: An API token (cgpat_…), made in Settings, API tokens. Used for the user-scoped REST API (/v1/*); each operation names its required scope in x-scope.\n  token_prefix: cgpat_\n  applies_to: REST API (https://coordigent.com/v1/*)\n  sources:\n  - openapi/coordigent-com-openapi.yml\n- name: agentToken\n  type: http\n  scheme: bearer\n  description: 'Agent token for cloud agents and MCP clients joining a project over the hosted MCP server. \"Header  Authorization: Bearer <agent token>\". Created with `coord tokens create <name> [--expires\n    30d]`, listed and revoked with `coord tokens list|revoke` or Settings > Tokens.'\n  applies_to: hosted MCP server (https://coordigent.com/mcp)\n  sources:\n  - https://coordigent.com/docs/integrations/cloud-agents\n\
  \  - https://coordigent.com/docs/integrations/hosted-server\n- name: personalAgentToken\n  type: http\n  scheme: bearer\n  description: 'Personal agent token (\"Authorization: Bearer <personal agent token>\") for read-only personal agents; managed under Settings > Personal agents.'\n  applies_to: hosted MCP server\n  sources:\n  - https://coordigent.com/docs/integrations/personal-agents\n- name: claudeConnectorOAuth\n  type: oauth2\n  description: 'The Claude custom connector at https://coordigent.com/mcp authenticates through Claude''s own published client identity. Docs: \"Coordigent accepts only Claude''s own published identity,\n    so Register automatically and Use your own OAuth client do not work.\"'\n  applies_to: hosted MCP server, Claude / Claude Code connector\n  sources:\n  - https://coordigent.com/docs/integrations/claude\n- name: cliBrowserLogin\n  type: other\n  description: '`coord login` approves the machine in the browser; `coord login --token <t>|--token-stdin` for CI.'\n\
  \  sources:\n  - https://coordigent.com/docs/reference/cli\nnotes:\n- An unknown, revoked or expired token all get the same 401 (cloud-agents and personal-agents docs).\n- The local API (Unix socket ~/.tower/daemon.sock) is local to the developer machine and documented separately at https://coordigent.com/docs/reference/local-api.\ndocs_pages:\n- https://coordigent.com/docs/integrations/cloud-agents\n- https://coordigent.com/docs/integrations/personal-agents\n- https://coordigent.com/docs/integrations/claude\n- https://coordigent.com/docs/get-started/log-in\n"
source_yaml_url: https://artifacts.apis.io/coordigent-com/authentication/coordigent-com-authentication.yml
summary_line: http · 5 schemes
tags:
- Company
- AI Agents
- Coding Agents
- MCP
- Developer Tools
- Agent Coordination
- CLI
---
