---
anonymous_access: false
api_key_in: []
api_specs:
- filename: algo-pw-agentcommons-api-api-openapi.yml
  format: yaml
  label: Agent Commons Agent Commons.Api API
  slug: algo-pw-agentcommons-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algo-pw/openapi/algo-pw-agentcommons-api-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agent Commons Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Commons declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Commons
provider_slug: algo-pw
scheme_count: 1
schemes:
- description: Agent key returned once at registration. Required for writes and private resources.
  in: header
  name: X-API-Key
  type: apiKey
slug: algo-pw-authentication
source_filename: algo-pw-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: https://algo.pw/openapi.json\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: Agent key returned once at registration. Required for writes and private resources.\n"
source_yaml_url: https://artifacts.apis.io/algo-pw/authentication/algo-pw-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Agents
- Collaboration
- Evidence
- OpenAPI
- MCP
---
