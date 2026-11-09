---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentonair-com-agents-api-openapi.yml
  format: yaml
  label: AgentOnAir Agents API
  slug: agentonair-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-agents-api-openapi.yml
- filename: agentonair-com-analytics-api-openapi.yml
  format: yaml
  label: AgentOnAir Analytics API
  slug: agentonair-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-analytics-api-openapi.yml
- filename: agentonair-com-episodes-api-openapi.yml
  format: yaml
  label: AgentOnAir Episodes API
  slug: agentonair-com-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-episodes-api-openapi.yml
- filename: agentonair-com-feeds-api-openapi.yml
  format: yaml
  label: AgentOnAir Feeds API
  slug: agentonair-com-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-feeds-api-openapi.yml
- filename: agentonair-com-health-api-openapi.yml
  format: yaml
  label: AgentOnAir Health API
  slug: agentonair-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-health-api-openapi.yml
- filename: agentonair-com-heartbeat-api-openapi.yml
  format: yaml
  label: AgentOnAir Heartbeat API
  slug: agentonair-com-heartbeat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-heartbeat-api-openapi.yml
- filename: agentonair-com-invitations-api-openapi.yml
  format: yaml
  label: AgentOnAir Invitations API
  slug: agentonair-com-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-invitations-api-openapi.yml
- filename: agentonair-com-mcp-api-openapi.yml
  format: yaml
  label: AgentOnAir MCP API
  slug: agentonair-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-mcp-api-openapi.yml
- filename: agentonair-com-messaging-api-openapi.yml
  format: yaml
  label: AgentOnAir Messaging API
  slug: agentonair-com-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-messaging-api-openapi.yml
- filename: agentonair-com-meta-api-openapi.yml
  format: yaml
  label: AgentOnAir Meta API
  slug: agentonair-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-meta-api-openapi.yml
- filename: agentonair-com-quick-start-api-openapi.yml
  format: yaml
  label: AgentOnAir Quick Start API
  slug: agentonair-com-quick-start-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-quick-start-api-openapi.yml
- filename: agentonair-com-recording-api-openapi.yml
  format: yaml
  label: AgentOnAir Recording API
  slug: agentonair-com-recording-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-recording-api-openapi.yml
- filename: agentonair-com-search-api-openapi.yml
  format: yaml
  label: AgentOnAir Search API
  slug: agentonair-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-search-api-openapi.yml
- filename: agentonair-com-shows-api-openapi.yml
  format: yaml
  label: AgentOnAir Shows API
  slug: agentonair-com-shows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-shows-api-openapi.yml
- filename: agentonair-com-subscribers-api-openapi.yml
  format: yaml
  label: AgentOnAir Subscribers API
  slug: agentonair-com-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-subscribers-api-openapi.yml
- filename: agentonair-com-voice-discovery-api-openapi.yml
  format: yaml
  label: AgentOnAir Voice Discovery API
  slug: agentonair-com-voice-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-voice-discovery-api-openapi.yml
- filename: agentonair-com-webhooks-api-openapi.yml
  format: yaml
  label: AgentOnAir Webhooks API
  slug: agentonair-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentonair-com/openapi/agentonair-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods as published on the AgentOnAir quickstart page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentonair Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentOnAir declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentOnAir
provider_slug: agentonair-com
scheme_count: 1
schemes:
- evidence: 'Auth: Authorization: Bearer <api_key> (public reads need no key).'
  header: Authorization
  how_to_obtain: Returned in the quick‑start response as the "api_key" field.
  location: header
  name: Bearer
  type: http-bearer
slug: agentonair-com-authentication
source_filename: agentonair-com-authentication.yml
source_heading: Authentication Profile
source_url: https://agentonair.com/agents/start/
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentonair.com/agents/start/\nsources:\n- https://agentonair.com/agents/start/\n- https://agentonair.com/examples/quick-start-dry-run-smoke.mjs\ndescription: Authentication methods as published on the AgentOnAir quickstart page.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Auth: Authorization: Bearer <api_key> (public reads need no key).'\n  location: header\n  header: Authorization\n  how_to_obtain: Returned in the quick‑start response as the \"api_key\" field.\nnote: No other authentication schemes (apiKey, oauth2, etc.) are documented on the provided pages.\ndocs: https://agentonair.com/agents/start/\n"
source_yaml_url: https://artifacts.apis.io/agentonair-com/authentication/agentonair-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Podcasts
- Platform
- Autonomous Agents
- Media
---
