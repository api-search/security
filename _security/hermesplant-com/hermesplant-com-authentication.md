---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hermesplant-com-action-safety-api-openapi.yml
  format: yaml
  label: Hermes Plant Action Safety API
  slug: hermesplant-com-action-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-action-safety-api-openapi.yml
- filename: hermesplant-com-agent-commerce-assurance-api-openapi.yml
  format: yaml
  label: Hermes Plant Agent Commerce Assurance API
  slug: hermesplant-com-agent-commerce-assurance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-agent-commerce-assurance-api-openapi.yml
- filename: hermesplant-com-agent-safety-api-openapi.yml
  format: yaml
  label: Hermes Plant Agent Safety API
  slug: hermesplant-com-agent-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-agent-safety-api-openapi.yml
- filename: hermesplant-com-agent-spend-api-openapi.yml
  format: yaml
  label: Hermes Plant Agent Spend API
  slug: hermesplant-com-agent-spend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-agent-spend-api-openapi.yml
- filename: hermesplant-com-assurance-api-openapi.yml
  format: yaml
  label: Hermes Plant Assurance API
  slug: hermesplant-com-assurance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-assurance-api-openapi.yml
- filename: hermesplant-com-billing-portal-api-openapi.yml
  format: yaml
  label: Hermes Plant Billing Portal API
  slug: hermesplant-com-billing-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-billing-portal-api-openapi.yml
- filename: hermesplant-com-catalog-api-openapi.yml
  format: yaml
  label: Hermes Plant Catalog API
  slug: hermesplant-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-catalog-api-openapi.yml
- filename: hermesplant-com-checkout-api-openapi.yml
  format: yaml
  label: Hermes Plant Checkout API
  slug: hermesplant-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-checkout-api-openapi.yml
- filename: hermesplant-com-content-api-openapi.yml
  format: yaml
  label: Hermes Plant Content API
  slug: hermesplant-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-content-api-openapi.yml
- filename: hermesplant-com-email-api-openapi.yml
  format: yaml
  label: Hermes Plant Email API
  slug: hermesplant-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-email-api-openapi.yml
- filename: hermesplant-com-finance-api-openapi.yml
  format: yaml
  label: Hermes Plant Finance API
  slug: hermesplant-com-finance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-finance-api-openapi.yml
- filename: hermesplant-com-health-api-openapi.yml
  format: yaml
  label: Hermes Plant Health API
  slug: hermesplant-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-health-api-openapi.yml
- filename: hermesplant-com-investment-analysis-api-openapi.yml
  format: yaml
  label: Hermes Plant Investment Analysis API
  slug: hermesplant-com-investment-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-investment-analysis-api-openapi.yml
- filename: hermesplant-com-mcp-api-openapi.yml
  format: yaml
  label: Hermes Plant MCP API
  slug: hermesplant-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-mcp-api-openapi.yml
- filename: hermesplant-com-portfolio-risk-analysis-api-openapi.yml
  format: yaml
  label: Hermes Plant Portfolio Risk Analysis API
  slug: hermesplant-com-portfolio-risk-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-portfolio-risk-analysis-api-openapi.yml
- filename: hermesplant-com-purchase-api-openapi.yml
  format: yaml
  label: Hermes Plant Purchase API
  slug: hermesplant-com-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-purchase-api-openapi.yml
- filename: hermesplant-com-wallet-risk-scoring-api-openapi.yml
  format: yaml
  label: Hermes Plant Wallet Risk Scoring API
  slug: hermesplant-com-wallet-risk-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-wallet-risk-scoring-api-openapi.yml
- filename: hermesplant-com-x402-api-openapi.yml
  format: yaml
  label: Hermes Plant X402 API
  slug: hermesplant-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-x402-api-openapi.yml
auth_types: []
description: Authentication schemes described on the page
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hermes Plant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hermes Plant declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hermes Plant
provider_slug: hermesplant-com
scheme_count: 2
schemes:
- evidence: API-key authentication An API key is a long-lived secret a human generates in a dashboard, stores securely, and rotates over time.
  name: API key
  type: apiKey
- evidence: 'x402 carries no credential: the caller proves it paid by signing a USDC-on-Base authorization for the exact price in the 402 challenge, then retries.'
  name: x402 per-request payment
  type: other
slug: hermesplant-com-authentication
source_filename: hermesplant-com-authentication.yml
source_heading: Authentication Profile
source_url: https://hermesplant.com/compare/x402-vs-api-keys
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hermesplant.com/compare/x402-vs-api-keys\nsources:\n- https://hermesplant.com/compare/x402-vs-api-keys\ndescription: Authentication schemes described on the page\nschemes:\n- type: apiKey\n  name: API key\n  evidence: API-key authentication An API key is a long-lived secret a human generates in a dashboard, stores securely, and rotates over time.\n- type: other\n  name: x402 per-request payment\n  evidence: 'x402 carries no credential: the caller proves it paid by signing a USDC-on-Base authorization for the exact price in the 402 challenge,\n    then retries.'\ndocs: https://hermesplant.com/compare/x402-vs-api-keys\n"
source_yaml_url: https://artifacts.apis.io/hermesplant-com/authentication/hermesplant-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Agent Safety
- Finance
- Compliance
- Automation
---
