---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentping-io-openapi-generated.yml
  format: yaml
  label: Agent Ping API
  slug: agentping-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentping-io/openapi/_ae-authored/agentping-io-openapi-generated.yml
auth_types: []
description: Authentication schemes for Agent Ping API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Agentping Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Ping declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Ping
provider_slug: agentping-io
scheme_count: 3
schemes:
- evidence: 'Authorization header Authorization: Bearer apk_eu_018f3a2b9c1d7e8fa4b9c2d7e8f1a3b6 Preferred for SDKs and any API key.'
  header: Authorization
  how_to_obtain: Issued from the agent's settings page in the dashboard.
  location: header
  name: Team API key
  type: apiKey
- evidence: 'X-AgentPing-Key header X-AgentPing-Key: ping_eu_018f3a2b9c1d7e8fa4b9c2d7e8f1a3b6 Alias of the above. Use when a proxy strips Authorization.'
  header: X-AgentPing-Key
  how_to_obtain: Issued from the agent's settings page in the dashboard.
  location: header
  name: Ping token
  type: apiKey
- evidence: ?key= query parameter https://eu.ingest.agentping.io/v1/ping?key=ping_eu_...&agent=daily-summary Allowed only on GET /v1/ping . Never put apk_ keys here.
  how_to_obtain: Issued from the agent's settings page in the dashboard.
  location: query
  name: Ping token (query)
  type: apiKey
slug: agentping-io-authentication
source_filename: agentping-io-authentication.yml
source_heading: Authentication Profile
source_url: https://agentping.io/docs/api/auth
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentping.io/docs/api/auth\nsources:\n- https://agentping.io/docs/api/auth\n- https://agentping.io/token-counter\n- https://agentping.io/token-bill-too-high\n- https://agentping.io/blog/anatomy-of-an-8900-token-bill\ndescription: Authentication schemes for Agent Ping API\nschemes:\n- type: apiKey\n  name: Team API key\n  evidence: 'Authorization header Authorization: Bearer apk_eu_018f3a2b9c1d7e8fa4b9c2d7e8f1a3b6 Preferred for SDKs and any API key.'\n  location: header\n  header: Authorization\n  how_to_obtain: Issued from the agent's settings page in the dashboard.\n- type: apiKey\n  name: Ping token\n  evidence: 'X-AgentPing-Key header X-AgentPing-Key: ping_eu_018f3a2b9c1d7e8fa4b9c2d7e8f1a3b6 Alias of the above. Use when a proxy strips Authorization.'\n  location: header\n  header: X-AgentPing-Key\n  how_to_obtain: Issued from the agent's settings page in the dashboard.\n\
  - type: apiKey\n  name: Ping token (query)\n  evidence: ?key= query parameter https://eu.ingest.agentping.io/v1/ping?key=ping_eu_...&agent=daily-summary Allowed only on GET /v1/ping . Never\n    put apk_ keys here.\n  location: query\n  how_to_obtain: Issued from the agent's settings page in the dashboard.\ndocs: https://agentping.io/docs/api/auth\n"
source_yaml_url: https://artifacts.apis.io/agentping-io/authentication/agentping-io-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Observability
- Monitoring
- Cost Management
- Software-as-a-Service
---
