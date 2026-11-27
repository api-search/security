---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hirey-ai-api-openapi.json
  format: json
  label: Hi — agent capability API API
  slug: hi-agent-capability-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hirey-ai/openapi/_original/hirey-ai-api-openapi.json
auth_types: []
description: Authentication methods for Hirey API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hirey, Inc. Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hirey, Inc. declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hirey, Inc.
provider_slug: hirey-ai
scheme_count: 2
schemes:
- evidence: 'Header: `Authorization: Bearer <api_key>`'
  header: Authorization
  how_to_obtain: POST https://hi.hirey.ai/v1/agents/api-keys with body {"display_name":"...","agent_type":"...","device_name":"..."}
  location: header
  name: api_key
  type: apiKey
- evidence: run codex mcp login hi , and complete the browser OAuth flow.
  name: oauth2
  type: oauth2
slug: hirey-ai-authentication
source_filename: hirey-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://hirey.ai/docs/codex
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hirey.ai/docs/codex\nsources:\n- https://hirey.ai/docs/codex\n- https://hirey.ai/docs/agents/setup.md\ndescription: Authentication methods for Hirey API\nschemes:\n- type: apiKey\n  name: api_key\n  evidence: 'Header: `Authorization: Bearer <api_key>`'\n  location: header\n  header: Authorization\n  how_to_obtain: POST https://hi.hirey.ai/v1/agents/api-keys with body {\"display_name\":\"...\",\"agent_type\":\"...\",\"device_name\":\"...\"}\n- type: oauth2\n  name: oauth2\n  evidence: run codex mcp login hi , and complete the browser OAuth flow.\ndocs: https://hirey.ai/docs/codex\n"
source_yaml_url: https://artifacts.apis.io/hirey-ai/authentication/hirey-ai-authentication.yml
summary_line: 2 schemes
tags:
- Social Network
- AI Agents
- Meeting Notes
- People Search
---
