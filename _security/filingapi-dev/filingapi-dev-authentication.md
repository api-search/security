---
anonymous_access: false
api_key_in: []
api_specs:
- filename: filingapi-dev-admin-api-openapi.yml
  format: yaml
  label: FilingAPI Admin API
  slug: filingapi-dev-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-admin-api-openapi.yml
- filename: filingapi-dev-calendar-api-openapi.yml
  format: yaml
  label: FilingAPI Calendar API
  slug: filingapi-dev-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-calendar-api-openapi.yml
- filename: filingapi-dev-checkout-api-openapi.yml
  format: yaml
  label: FilingAPI Checkout API
  slug: filingapi-dev-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-checkout-api-openapi.yml
- filename: filingapi-dev-company-api-openapi.yml
  format: yaml
  label: FilingAPI Company API
  slug: filingapi-dev-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-company-api-openapi.yml
- filename: filingapi-dev-earnings-filings-api-api-openapi.yml
  format: yaml
  label: FilingAPI Earnings & Filings API
  slug: filingapi-dev-earnings-filings-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-earnings-filings-api-api-openapi.yml
- filename: filingapi-dev-favicon-ico-api-openapi.yml
  format: yaml
  label: FilingAPI Favicon.ico API
  slug: filingapi-dev-favicon-ico-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-favicon-ico-api-openapi.yml
- filename: filingapi-dev-filings-api-openapi.yml
  format: yaml
  label: FilingAPI Filings API
  slug: filingapi-dev-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-filings-api-openapi.yml
- filename: filingapi-dev-health-api-openapi.yml
  format: yaml
  label: FilingAPI Health API
  slug: filingapi-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-health-api-openapi.yml
- filename: filingapi-dev-insiders-api-openapi.yml
  format: yaml
  label: FilingAPI Insiders API
  slug: filingapi-dev-insiders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-insiders-api-openapi.yml
- filename: filingapi-dev-mcp-api-openapi.yml
  format: yaml
  label: FilingAPI MCP API
  slug: filingapi-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-mcp-api-openapi.yml
- filename: filingapi-dev-model-api-openapi.yml
  format: yaml
  label: FilingAPI Model API
  slug: filingapi-dev-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-model-api-openapi.yml
- filename: filingapi-dev-sectors-api-openapi.yml
  format: yaml
  label: FilingAPI Sectors API
  slug: filingapi-dev-sectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-sectors-api-openapi.yml
- filename: filingapi-dev-signals-api-openapi.yml
  format: yaml
  label: FilingAPI Signals API
  slug: filingapi-dev-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-signals-api-openapi.yml
- filename: filingapi-dev-signup-api-openapi.yml
  format: yaml
  label: FilingAPI Signup API
  slug: filingapi-dev-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-signup-api-openapi.yml
- filename: filingapi-dev-transcripts-api-openapi.yml
  format: yaml
  label: FilingAPI Transcripts API
  slug: filingapi-dev-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-transcripts-api-openapi.yml
- filename: filingapi-dev-verify-api-openapi.yml
  format: yaml
  label: FilingAPI Verify API
  slug: filingapi-dev-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-verify-api-openapi.yml
- filename: filingapi-dev-webhooks-api-openapi.yml
  format: yaml
  label: FilingAPI Webhooks API
  slug: filingapi-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Filingapi Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: FilingAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FilingAPI
provider_slug: filingapi-dev
scheme_count: 1
schemes:
- description: API key passed in the X-API-Key request header. Keys are obtained by starting a free trial from the homepage.
  evidence: 'curl https://filingapi.dev/v1/filings/AAPL -H "X-API-Key: YOUR_KEY"'
  in: header
  name: X-API-Key
  type: apiKey
slug: filingapi-dev-authentication
source_filename: filingapi-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filingapi.dev/\ndocs: https://filingapi.dev/docs\nname: FilingAPI authentication\nschemes:\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: >-\n      API key passed in the X-API-Key request header. Keys are obtained by\n      starting a free trial from the homepage.\n    evidence: |-\n      curl https://filingapi.dev/v1/filings/AAPL -H \"X-API-Key: YOUR_KEY\"\nnote: >-\n  The published OpenAPI document (https://filingapi.dev/openapi.json) does not\n  declare any securitySchemes; the X-API-Key header authentication scheme is\n  stated on the homepage code samples and MCP integration snippet.\n"
source_yaml_url: https://artifacts.apis.io/filingapi-dev/authentication/filingapi-dev-authentication.yml
summary_line: 1 scheme
tags:
- Financial Data
- SEC Filings
- Earnings
- Macro Economic
- Sentiment Analysis
- Quantitative Finance
- MCP Server
- REST API
---
