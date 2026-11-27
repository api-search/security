---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: costkits-com-bill-analysis-api-openapi.yml
  format: yaml
  label: CostKits Bill Analysis API
  slug: costkits-com-bill-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costkits-com/openapi/costkits-com-bill-analysis-api-openapi.yml
- filename: costkits-com-cost-estimation-api-openapi.yml
  format: yaml
  label: CostKits Cost Estimation API
  slug: costkits-com-cost-estimation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costkits-com/openapi/costkits-com-cost-estimation-api-openapi.yml
- filename: costkits-com-coverage-rules-api-openapi.yml
  format: yaml
  label: CostKits Coverage Rules API
  slug: costkits-com-coverage-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costkits-com/openapi/costkits-com-coverage-rules-api-openapi.yml
- filename: costkits-com-demo-api-openapi.yml
  format: yaml
  label: CostKits Demo API
  slug: costkits-com-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costkits-com/openapi/costkits-com-demo-api-openapi.yml
- filename: costkits-com-procedure-ontology-api-openapi.yml
  format: yaml
  label: CostKits Procedure Ontology API
  slug: costkits-com-procedure-ontology-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costkits-com/openapi/costkits-com-procedure-ontology-api-openapi.yml
- filename: costkits-com-provider-graph-api-openapi.yml
  format: yaml
  label: CostKits Provider Graph API
  slug: costkits-com-provider-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costkits-com/openapi/costkits-com-provider-graph-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CostKits Authentication
name_suffix: Authentication
oauth_flows: []
overview: CostKits secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CostKits
provider_slug: costkits-com
scheme_count: 1
schemes:
- description: 'Bearer token: Authorization: Bearer YOUR_API_KEY. Keys look like ck_... -- the prefix is safe to log, the full key is not.'
  format: 'Authorization: Bearer YOUR_API_KEY'
  in: header
  key_prefix: ck_
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/costkits-com-openapi.yml
  - https://github.com/costkits/costkits-api/blob/main/docs/authentication.md
  type: apiKey
  unauthenticated_operations:
  - demoEstimate
slug: costkits-com-authentication
source_filename: costkits-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://github.com/costkits/costkits-api/blob/main/docs/authentication.md\ndocs: https://github.com/costkits/costkits-api/blob/main/docs/authentication.md\nstatus: retired\nnote: 'The costkits-api README states \"Retired 2026-10-16. CostKits no longer issues API keys or sells Builder/Pro plans.\"\n  The successor MCP server (https://mcp.costkits.com/mcp) is documented at https://www.costkits.com/agents/ as \"No account, no key.\"'\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer YOUR_API_KEY'\n  key_prefix: ck_\n  description: 'Bearer token: Authorization: Bearer YOUR_API_KEY. Keys look like ck_... -- the prefix is safe to log, the full key is not.'\n  unauthenticated_operations:\n  - demoEstimate\n  sources:\n  - openapi/costkits-com-openapi.yml\n  - https://github.com/costkits/costkits-api/blob/main/docs/authentication.md\n\
  failure_modes:\n- {status: 401, meaning: Missing or invalid key}\n- {status: 403, meaning: 'Key is valid, plan too low for this endpoint'}\n- {status: 429, meaning: Monthly quota exhausted or per-minute limit hit}\n"
source_yaml_url: https://artifacts.apis.io/costkits-com/authentication/costkits-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Healthcare
- Medical Billing
- Healthcare Costs
- Price Transparency
- Caregivers
- Insurance
- MCP
---
