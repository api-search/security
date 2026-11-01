---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gatherhq-com-agents-api-openapi.yml
  format: yaml
  label: Gather Agents API
  slug: gatherhq-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-agents-api-openapi.yml
- filename: gatherhq-com-dimensions-api-openapi.yml
  format: yaml
  label: Gather Dimensions API
  slug: gatherhq-com-dimensions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-dimensions-api-openapi.yml
- filename: gatherhq-com-health-api-openapi.yml
  format: yaml
  label: Gather Health API
  slug: gatherhq-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-health-api-openapi.yml
- filename: gatherhq-com-mcp-api-openapi.yml
  format: yaml
  label: Gather MCP API
  slug: gatherhq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-mcp-api-openapi.yml
- filename: gatherhq-com-questions-api-openapi.yml
  format: yaml
  label: Gather Questions API
  slug: gatherhq-com-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-questions-api-openapi.yml
- filename: gatherhq-com-reviews-api-openapi.yml
  format: yaml
  label: Gather Reviews API
  slug: gatherhq-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-reviews-api-openapi.yml
- filename: gatherhq-com-sources-api-openapi.yml
  format: yaml
  label: Gather Sources API
  slug: gatherhq-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-sources-api-openapi.yml
- filename: gatherhq-com-stats-api-openapi.yml
  format: yaml
  label: Gather Stats API
  slug: gatherhq-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-stats-api-openapi.yml
- filename: gatherhq-com-tools-api-openapi.yml
  format: yaml
  label: Gather Tools API
  slug: gatherhq-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-tools-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Gatherhq Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gather declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Gather
provider_slug: gatherhq-com
scheme_count: 3
schemes:
- description: Bearer token authentication.
  in: header
  name: Authorization
  type: apiKey
- description: API key authentication.
  in: header
  name: x-api-key
  type: apiKey
- description: Ed25519-signed writes as described in OpenAPI.
  scheme: ed25519
  type: http
slug: gatherhq-com-authentication
source_filename: gatherhq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://www.gatherhq.com/docs\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token authentication.\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API key authentication.\n  - type: http\n    scheme: ed25519\n    description: Ed25519-signed writes as described in OpenAPI.\n"
source_yaml_url: https://artifacts.apis.io/gatherhq-com/authentication/gatherhq-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Buyer-Intelligence
- Market-Research
- GTM-Tools
- SaaS
---
