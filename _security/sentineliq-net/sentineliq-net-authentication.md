---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sentineliq-net-agent-api-api-openapi.yml
  format: yaml
  label: sentineliq-net Agent API
  slug: sentineliq-net-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-agent-api-api-openapi.yml
- filename: sentineliq-net-mcp-api-openapi.yml
  format: yaml
  label: sentineliq-net MCP API
  slug: sentineliq-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-mcp-api-openapi.yml
- filename: sentineliq-net-property-research-api-openapi.yml
  format: yaml
  label: sentineliq-net Property Research API
  slug: sentineliq-net-property-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-property-research-api-openapi.yml
- filename: sentineliq-net-public-api-openapi.yml
  format: yaml
  label: sentineliq-net Public API
  slug: sentineliq-net-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-public-api-openapi.yml
- filename: sentineliq-net-seller-workflows-api-openapi.yml
  format: yaml
  label: sentineliq-net Seller Workflows API
  slug: sentineliq-net-seller-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentineliq-net/openapi/sentineliq-net-seller-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Sentineliq Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: sentineliq-net secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: sentineliq-net
provider_slug: sentineliq-net
scheme_count: 1
schemes:
- bearerFormat: agk_...
  description: 'SENTINEL Developer API key (Authorization: Bearer agk_...). X-API-Key: agk_... is accepted as an equivalent.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/agent-api.json
  type: http
slug: sentineliq-net-authentication
source_filename: sentineliq-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/agent-api.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: agk_...\n  description: 'SENTINEL Developer API key (Authorization: Bearer agk_...). X-API-Key: agk_...\n    is accepted as an equivalent.'\n  sources:\n  - openapi/agent-api.json\n"
source_yaml_url: https://artifacts.apis.io/sentineliq-net/authentication/sentineliq-net-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Real Estate
- Data API
- Washington
- AI Integration
---
