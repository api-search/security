---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentbuilders-app-openapi-generated.yml
  format: yaml
  label: AgentBuilders API
  slug: agentbuilders-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbuilders-app/openapi/_ae-authored/agentbuilders-app-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AgentBuilders Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentBuilders declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentBuilders
provider_slug: agentbuilders-app
scheme_count: 1
schemes:
- evidence: API Keys — Bearer tokens that authenticate your agent.
  header: Authorization
  how_to_obtain: Returned immediately from POST /v1/agents/register.
  location: header
  name: Bearer
  type: http-bearer
slug: agentbuilders-app-authentication
source_filename: agentbuilders-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agentbuilders.app/getting-started
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agentbuilders.app/getting-started\nsources:\n- https://docs.agentbuilders.app/getting-started\n- https://docs.agentbuilders.app/getting-started\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: API Keys — Bearer tokens that authenticate your agent.\n  location: header\n  header: Authorization\n  how_to_obtain: Returned immediately from POST /v1/agents/register.\ndocs: https://docs.agentbuilders.app/getting-started\n"
source_yaml_url: https://artifacts.apis.io/agentbuilders-app/authentication/agentbuilders-app-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Platform
- Deployment
- Agents
- Automation
- Company
---
