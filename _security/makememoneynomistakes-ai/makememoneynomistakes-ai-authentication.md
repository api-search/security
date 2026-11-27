---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: makememoneynomistakes-ai-agents-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Agents API
  slug: makememoneynomistakes-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-agents-api-openapi.yml
- filename: makememoneynomistakes-ai-bouncer-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Bouncer API
  slug: makememoneynomistakes-ai-bouncer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-bouncer-api-openapi.yml
- filename: makememoneynomistakes-ai-directory-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Directory API
  slug: makememoneynomistakes-ai-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-directory-api-openapi.yml
- filename: makememoneynomistakes-ai-export-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Export API
  slug: makememoneynomistakes-ai-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-export-api-openapi.yml
- filename: makememoneynomistakes-ai-health-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Health API
  slug: makememoneynomistakes-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-health-api-openapi.yml
- filename: makememoneynomistakes-ai-makememoneynomistakes-ai-reputation-and-fraud-checks-for-erc-8004-agents-on-base-api-openapi.yml
  format: yaml
  label: 'Make Money No Mistakes AI Makememoneynomistakes.ai: Reputation And Fraud Checks For ERC 8004 Agents On Base API'
  slug: makememoneynomistakes-ai-makememoneynomistakes-ai-reputation-and-fraud-checks-for-erc-8004-agents-on-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-makememoneynomistakes-ai-reputation-and-fraud-checks-for-erc-8004-agents-on-base-api-openapi.yml
- filename: makememoneynomistakes-ai-mcp-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI MCP API
  slug: makememoneynomistakes-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-mcp-api-openapi.yml
- filename: makememoneynomistakes-ai-pass-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Pass API
  slug: makememoneynomistakes-ai-pass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-pass-api-openapi.yml
- filename: makememoneynomistakes-ai-pathways-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Pathways API
  slug: makememoneynomistakes-ai-pathways-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-pathways-api-openapi.yml
- filename: makememoneynomistakes-ai-payments-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Payments API
  slug: makememoneynomistakes-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-payments-api-openapi.yml
- filename: makememoneynomistakes-ai-platform-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Platform API
  slug: makememoneynomistakes-ai-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-platform-api-openapi.yml
- filename: makememoneynomistakes-ai-results-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Results API
  slug: makememoneynomistakes-ai-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-results-api-openapi.yml
- filename: makememoneynomistakes-ai-revenue-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Revenue API
  slug: makememoneynomistakes-ai-revenue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-revenue-api-openapi.yml
- filename: makememoneynomistakes-ai-search-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Search API
  slug: makememoneynomistakes-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-search-api-openapi.yml
- filename: makememoneynomistakes-ai-sellkit-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Sellkit API
  slug: makememoneynomistakes-ai-sellkit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-sellkit-api-openapi.yml
- filename: makememoneynomistakes-ai-stats-api-openapi.yml
  format: yaml
  label: Make Money No Mistakes AI Stats API
  slug: makememoneynomistakes-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makememoneynomistakes-ai/openapi/makememoneynomistakes-ai-stats-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Make Money No Mistakes AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Make Money No Mistakes AI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Make Money No Mistakes AI
provider_slug: makememoneynomistakes-ai
scheme_count: 2
schemes:
- description: Purchased call-bundle token; not an account API key.
  in: header
  name: CallPass
  parameter: X-MMNM-Pass
  sources:
  - openapi/makememoneynomistakes-ai-openapi.json
  type: apiKey
- bearerFormat: MMNM call-bundle pass
  description: Optional pass for MCP only. No OAuth login flow.
  name: McpPass
  scheme: bearer
  sources:
  - openapi/makememoneynomistakes-ai-openapi.json
  type: http
slug: makememoneynomistakes-ai-authentication
source_filename: makememoneynomistakes-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/makememoneynomistakes-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: CallPass\n  type: apiKey\n  in: header\n  parameter: X-MMNM-Pass\n  description: Purchased call-bundle token; not an account API key.\n  sources:\n  - openapi/makememoneynomistakes-ai-openapi.json\n- name: McpPass\n  type: http\n  scheme: bearer\n  bearerFormat: MMNM call-bundle pass\n  description: Optional pass for MCP only. No OAuth login flow.\n  sources:\n  - openapi/makememoneynomistakes-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/makememoneynomistakes-ai/authentication/makememoneynomistakes-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Reputation
- Blockchain
- Base
- ERC-8004
---
