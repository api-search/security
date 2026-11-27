---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentic-endpoints-com-compress-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Compress API
  slug: agentic-endpoints-com-compress-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-compress-api-openapi.yml
- filename: agentic-endpoints-com-credits-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Credits API
  slug: agentic-endpoints-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-credits-api-openapi.yml
- filename: agentic-endpoints-com-meetings-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Meetings API
  slug: agentic-endpoints-com-meetings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-meetings-api-openapi.yml
- filename: agentic-endpoints-com-once-key-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Once Key API
  slug: agentic-endpoints-com-once-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-once-key-api-openapi.yml
- filename: agentic-endpoints-com-pdf-parse-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Pdf Parse API
  slug: agentic-endpoints-com-pdf-parse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-pdf-parse-api-openapi.yml
- filename: agentic-endpoints-com-reach-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Reach API
  slug: agentic-endpoints-com-reach-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-reach-api-openapi.yml
- filename: agentic-endpoints-com-scrape-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Scrape API
  slug: agentic-endpoints-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-scrape-api-openapi.yml
- filename: agentic-endpoints-com-vault-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Vault API
  slug: agentic-endpoints-com-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-vault-api-openapi.yml
- filename: agentic-endpoints-com-x402-api-openapi.yml
  format: yaml
  label: Agentic Endpoints X402 API
  slug: agentic-endpoints-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-x402-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Agentic Endpoints Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agentic Endpoints declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Agentic Endpoints
provider_slug: agentic-endpoints-com
scheme_count: 2
schemes:
- description: A prepaid or trial balance. Get one free with no wallet and no account at POST https://agentic-endpoints.com/credits/trial, or buy credit at POST https://agentic-endpoints.com/credits/buy. Each call is debited at the route's list price and nothing is signed per request.
  in: header
  name: X-Credit-Token
  type: apiKey
- description: A signed x402 payment authorising this one call, built from the challenge returned with HTTP 402. Requires a funded wallet on Base; the credit token does not.
  in: header
  name: X-PAYMENT
  type: apiKey
slug: agentic-endpoints-com-authentication
source_filename: agentic-endpoints-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agentic-endpoints-com-openapi.yml\nschemes:\n  - type: apiKey\n    name: X-Credit-Token\n    in: header\n    description: A prepaid or trial balance. Get one free with no wallet and no account at POST https://agentic-endpoints.com/credits/trial, or buy credit at POST https://agentic-endpoints.com/credits/buy. Each call is debited at the route's list price and nothing is signed per request.\n  - type: apiKey\n    name: X-PAYMENT\n    in: header\n    description: A signed x402 payment authorising this one call, built from the challenge returned with HTTP 402. Requires a funded wallet on Base; the credit token does not.\n"
source_yaml_url: https://artifacts.apis.io/agentic-endpoints-com/authentication/agentic-endpoints-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Agents
- Payments
- Micro-utilities
- Base
---
