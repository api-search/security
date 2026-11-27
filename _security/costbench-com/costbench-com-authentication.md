---
anonymous_access: true
api_key_in: []
api_specs:
- filename: costbench-com-compare-api-openapi.yml
  format: yaml
  label: CostBench Compare API
  slug: costbench-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-compare-api-openapi.yml
- filename: costbench-com-coverage-api-openapi.yml
  format: yaml
  label: CostBench Coverage API
  slug: costbench-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-coverage-api-openapi.yml
- filename: costbench-com-discover-api-openapi.yml
  format: yaml
  label: CostBench Discover API
  slug: costbench-com-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-discover-api-openapi.yml
- filename: costbench-com-history-api-openapi.yml
  format: yaml
  label: CostBench History API
  slug: costbench-com-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-history-api-openapi.yml
- filename: costbench-com-mcp-api-openapi.yml
  format: yaml
  label: CostBench MCP API
  slug: costbench-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-mcp-api-openapi.yml
- filename: costbench-com-pricing-api-openapi.yml
  format: yaml
  label: CostBench Pricing API
  slug: costbench-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-pricing-api-openapi.yml
- filename: costbench-com-tco-api-openapi.yml
  format: yaml
  label: CostBench Tco API
  slug: costbench-com-tco-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-tco-api-openapi.yml
- filename: costbench-com-usage-api-openapi.yml
  format: yaml
  label: CostBench Usage API
  slug: costbench-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costbench-com/openapi/costbench-com-usage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: CostBench Authentication
name_suffix: Authentication
oauth_flows: []
overview: CostBench declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CostBench
provider_slug: costbench-com
scheme_count: 1
schemes:
- applies_to: all /api/v2 endpoints and the MCP server at https://costbench.com/mcp
  description: No API key required today. CORS is open on all v2 endpoints.
  name: none
  type: none
slug: costbench-com-authentication
source_filename: costbench-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://costbench.com/api-docs/\ndocs: https://costbench.com/api-docs/\nsummary: The API is keyless. The docs state \"No API key required today.\" The OpenAPI 3.1 contract declares no securitySchemes. Access is limited by a per-IP rate limit and a fair-use daily allowance, not by credentials.\nschemes:\n- name: none\n  type: none\n  description: No API key required today. CORS is open on all v2 endpoints.\n  applies_to: all /api/v2 endpoints and the MCP server at https://costbench.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/costbench-com/authentication/costbench-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Software Pricing
- Software-as-a-Service
- Procurement
- Cost Intelligence
- Price Comparison
- Total Cost of Ownership
- MCP
---
