---
anonymous_access: true
api_key_in: []
api_specs:
- filename: areyoufoundbyai-com-openapi-generated.yml
  format: yaml
  label: Tech Horizon Labs API
  slug: areyoufoundbyai-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/areyoufoundbyai-com/openapi/_ae-authored/areyoufoundbyai-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Tech Horizon Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tech Horizon Labs declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Tech Horizon Labs
provider_slug: areyoufoundbyai-com
scheme_count: 4
schemes:
- description: Public free scan endpoint /api/scan requires no authentication.
  type: none
- description: Token for MCP server and console feeds.
  header: Authorization
  in: header
  name: monitor token
  type: apiKey
- description: Scoped agency key for network catalogue.
  header: Authorization
  in: header
  name: scoped key
  type: apiKey
- description: Payment per call for /api/agent/* endpoints.
  name: x402
  type: custom
slug: areyoufoundbyai-com-authentication
source_filename: areyoufoundbyai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://areyoufoundbyai.com/docs/api/authentication.md\nname: Are you found by AI? authentication\nschemes:\n  - type: none\n    description: Public free scan endpoint /api/scan requires no authentication.\n  - type: apiKey\n    name: monitor token\n    in: header\n    header: Authorization\n    description: Token for MCP server and console feeds.\n  - type: apiKey\n    name: scoped key\n    in: header\n    header: Authorization\n    description: Scoped agency key for network catalogue.\n  - type: custom\n    name: x402\n    description: Payment per call for /api/agent/* endpoints.\n"
source_yaml_url: https://artifacts.apis.io/areyoufoundbyai-com/authentication/areyoufoundbyai-com-authentication.yml
summary_line: 4 schemes
tags:
- Artificial Intelligence
- Growth
- Marketing
- SEO
- Australian
---
