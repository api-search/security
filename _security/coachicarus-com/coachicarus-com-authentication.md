---
anonymous_access: true
api_key_in: []
api_specs:
- filename: coachicarus-com-agent-api-openapi.yml
  format: yaml
  label: Coach Icarus Agent API
  slug: coachicarus-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coachicarus-com/openapi/coachicarus-com-agent-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Coach Icarus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coach Icarus declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Coach Icarus
provider_slug: coachicarus-com
scheme_count: 3
schemes:
- alternate_transport: 'Authorization: Bearer <personal API key>'
  applies_to: Hosted MCP server (https://api.coachicarus.com/mcp)
  description: Generate a key in the dashboard under Settings → API keys and send it as an X-API-Key header or a Bearer token. Keys are read-only, revocable at any time (revocation is immediate), and limited to ten active keys per account.
  header: X-API-Key
  in: header
  key_prefix: ick_live_
  name: PersonalApiKey
  type: apiKey
- applies_to: Account-specific Coach Icarus API endpoints (schema not published)
  description: Account-specific Coach Icarus API endpoints require a bearer access token issued by the Coach Icarus authentication flow.
  name: BearerAccessToken
  scheme: bearer
  type: http
- applies_to: GET /api/v1/agent
  description: The public agent discovery endpoint is read-only and does not require authentication.
  name: None
  type: none
slug: coachicarus-com-authentication
source_filename: coachicarus-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.coachicarus.com/developers/authentication\ndocs: https://www.coachicarus.com/developers/authentication\nnote: The published OpenAPI (public agent API, GET /api/v1/agent) declares no securitySchemes; the endpoint is documented as unauthenticated. Schemes below are read from the docs.\nschemes:\n- name: PersonalApiKey\n  type: apiKey\n  in: header\n  header: X-API-Key\n  applies_to: Hosted MCP server (https://api.coachicarus.com/mcp)\n  key_prefix: ick_live_\n  description: \"Generate a key in the dashboard under Settings → API keys and send it as an X-API-Key header or a Bearer token. Keys are read-only, revocable at any time (revocation is immediate), and limited to ten active keys per account.\"\n  alternate_transport: 'Authorization: Bearer <personal API key>'\n- name: BearerAccessToken\n  type: http\n  scheme: bearer\n  applies_to: Account-specific Coach Icarus API endpoints (schema not published)\n  description:\
  \ \"Account-specific Coach Icarus API endpoints require a bearer access token issued by the Coach Icarus authentication flow.\"\n- name: None\n  type: none\n  applies_to: GET /api/v1/agent\n  description: \"The public agent discovery endpoint is read-only and does not require authentication.\"\n"
source_yaml_url: https://artifacts.apis.io/coachicarus-com/authentication/coachicarus-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Running
- Fitness
- Coaching
- Garmin
- Health
- Wearables
- MCP
- AI Agents
---
