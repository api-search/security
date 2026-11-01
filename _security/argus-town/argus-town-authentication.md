---
anonymous_access: false
api_key_in: []
api_specs:
- filename: argus-town-alerts-api-openapi.yml
  format: yaml
  label: argus-town Alerts API
  slug: argus-town-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-alerts-api-openapi.yml
- filename: argus-town-connect-links-api-openapi.yml
  format: yaml
  label: argus-town Connect links API
  slug: argus-town-connect-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-connect-links-api-openapi.yml
- filename: argus-town-connections-api-openapi.yml
  format: yaml
  label: argus-town Connections API
  slug: argus-town-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-connections-api-openapi.yml
- filename: argus-town-events-api-openapi.yml
  format: yaml
  label: argus-town Events API
  slug: argus-town-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-events-api-openapi.yml
- filename: argus-town-negotiated-pricing-api-openapi.yml
  format: yaml
  label: argus-town Negotiated pricing API
  slug: argus-town-negotiated-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-negotiated-pricing-api-openapi.yml
- filename: argus-town-project-api-openapi.yml
  format: yaml
  label: argus-town Project API
  slug: argus-town-project-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-project-api-openapi.yml
- filename: argus-town-providers-api-openapi.yml
  format: yaml
  label: argus-town Providers API
  slug: argus-town-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-providers-api-openapi.yml
- filename: argus-town-spend-api-openapi.yml
  format: yaml
  label: argus-town Spend API
  slug: argus-town-spend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-spend-api-openapi.yml
- filename: argus-town-start-api-openapi.yml
  format: yaml
  label: argus-town Start API
  slug: argus-town-start-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-start-api-openapi.yml
- filename: argus-town-syncs-api-openapi.yml
  format: yaml
  label: argus-town Syncs API
  slug: argus-town-syncs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-syncs-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Argus Town Authentication
name_suffix: Authentication
oauth_flows: []
overview: argus-town declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: argus-town
provider_slug: argus-town
scheme_count: 3
schemes:
- description: Bearer token for API keys (type "api")
  in: header
  name: Authorization
  type: apiKey
- description: Bearer token for MCP keys (type "mcp")
  in: header
  name: Authorization
  type: apiKey
- description: HMAC-SHA256 signature for source secret, using X-Argus-Source, X-Argus-Timestamp, X-Argus-Signature headers
  scheme: hmac
  type: http
slug: argus-town-authentication
source_filename: argus-town-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://argus.town/docs/authentication\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token for API keys (type \"api\")\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token for MCP keys (type \"mcp\")\n  - type: http\n    scheme: hmac\n    description: HMAC-SHA256 signature for source secret, using X-Argus-Source, X-Argus-Timestamp, X-Argus-Signature headers\n"
source_yaml_url: https://artifacts.apis.io/argus-town/authentication/argus-town-authentication.yml
summary_line: 3 schemes
tags:
- Company
- API-Monitoring
- Cost-Management
- Developer-Tools
- MCP
---
