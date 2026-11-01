---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Agent Groundcrew API
  slug: agentgroundcrew-api
  spec_type: OpenAPI
  url: https://agentgroundcrew.com/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agentgroundcrew Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: agentgroundcrew-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: agentgroundcrew-com
provider_slug: agentgroundcrew-com
scheme_count: 1
schemes:
- description: 64-character random hex token chosen when submitting the request
  scheme: bearer
  type: http
slug: agentgroundcrew-com-authentication
source_filename: agentgroundcrew-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://agentgroundcrew.com/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    description: 64-character random hex token chosen when submitting the request\n"
source_yaml_url: https://artifacts.apis.io/agentgroundcrew-com/authentication/agentgroundcrew-com-authentication.yml
summary_line: 1 scheme
tags:
- Field Services
- Human Execution
- MCP
- Payments
- REST API
---
