---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentpay-so-acp-api-openapi.yml
  format: yaml
  label: AgentPay Labs ACP API
  slug: agentpay-so-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-acp-api-openapi.yml
- filename: agentpay-so-agentrank-api-openapi.yml
  format: yaml
  label: AgentPay Labs Agent Rank API
  slug: agentpay-so-agentrank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-agentrank-api-openapi.yml
- filename: agentpay-so-agents-api-openapi.yml
  format: yaml
  label: AgentPay Labs Agents API
  slug: agentpay-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-agents-api-openapi.yml
- filename: agentpay-so-ap2-api-openapi.yml
  format: yaml
  label: AgentPay Labs AP2 API
  slug: agentpay-so-ap2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-ap2-api-openapi.yml
- filename: agentpay-so-commerce-api-openapi.yml
  format: yaml
  label: AgentPay Labs Commerce API
  slug: agentpay-so-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-commerce-api-openapi.yml
- filename: agentpay-so-escrow-api-openapi.yml
  format: yaml
  label: AgentPay Labs Escrow API
  slug: agentpay-so-escrow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-escrow-api-openapi.yml
- filename: agentpay-so-health-api-openapi.yml
  format: yaml
  label: AgentPay Labs Health API
  slug: agentpay-so-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-health-api-openapi.yml
- filename: agentpay-so-marketplace-api-openapi.yml
  format: yaml
  label: AgentPay Labs Marketplace API
  slug: agentpay-so-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-marketplace-api-openapi.yml
- filename: agentpay-so-merchants-api-openapi.yml
  format: yaml
  label: AgentPay Labs Merchants API
  slug: agentpay-so-merchants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-merchants-api-openapi.yml
- filename: agentpay-so-payments-api-openapi.yml
  format: yaml
  label: AgentPay Labs Payments API
  slug: agentpay-so-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-payments-api-openapi.yml
- filename: agentpay-so-webhooks-api-openapi.yml
  format: yaml
  label: AgentPay Labs Webhooks API
  slug: agentpay-so-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpay-so/openapi/agentpay-so-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for AgentPay Labs API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AgentPay Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentPay Labs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentPay Labs
provider_slug: agentpay-so
scheme_count: 1
schemes:
- evidence: 'Pass your API key as Authorization: Bearer apk_...'
  header: Authorization
  how_to_obtain: Register via POST https://api.agentpay.so/api/merchants/register which returns an "apiKey" value.
  location: header
  name: API Key
  type: http-bearer
slug: agentpay-so-authentication
source_filename: agentpay-so-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agentpay.so/quickstart
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agentpay.so/quickstart\nsources:\n- https://docs.agentpay.so/quickstart\ndescription: Authentication schemes for AgentPay Labs API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Pass your API key as Authorization: Bearer apk_...'\n  location: header\n  header: Authorization\n  how_to_obtain: Register via POST https://api.agentpay.so/api/merchants/register which returns an \"apiKey\" value.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented on the page.\ndocs: https://docs.agentpay.so/quickstart\n"
source_yaml_url: https://artifacts.apis.io/agentpay-so/authentication/agentpay-so-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Research
- Robotics
- Automation
- Platform
---
