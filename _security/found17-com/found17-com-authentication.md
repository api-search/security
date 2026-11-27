---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: found17-com-compare-products-api-openapi.yml
  format: yaml
  label: Found17 Compare Products API
  slug: found17-com-compare-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-compare-products-api-openapi.yml
- filename: found17-com-health-api-openapi.yml
  format: yaml
  label: Found17 Health API
  slug: found17-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-health-api-openapi.yml
- filename: found17-com-quote-api-openapi.yml
  format: yaml
  label: Found17 Quote API
  slug: found17-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-quote-api-openapi.yml
- filename: found17-com-services-api-openapi.yml
  format: yaml
  label: Found17 Services API
  slug: found17-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-services-api-openapi.yml
- filename: found17-com-source-snapshot-api-openapi.yml
  format: yaml
  label: Found17 Source Snapshot API
  slug: found17-com-source-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-source-snapshot-api-openapi.yml
- filename: found17-com-source-watches-api-openapi.yml
  format: yaml
  label: Found17 Source Watches API
  slug: found17-com-source-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-source-watches-api-openapi.yml
- filename: found17-com-verify-claim-api-openapi.yml
  format: yaml
  label: Found17 Verify Claim API
  slug: found17-com-verify-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-verify-claim-api-openapi.yml
- filename: found17-com-web-qa-api-openapi.yml
  format: yaml
  label: Found17 Web Qa API
  slug: found17-com-web-qa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-web-qa-api-openapi.yml
- filename: found17-com-web-to-product-api-openapi.yml
  format: yaml
  label: Found17 Web To Product API
  slug: found17-com-web-to-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-web-to-product-api-openapi.yml
- filename: found17-com-website-audit-api-openapi.yml
  format: yaml
  label: Found17 Website Audit API
  slug: found17-com-website-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/found17-com/openapi/found17-com-website-audit-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Found17 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Found17 secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Found17
provider_slug: found17-com
scheme_count: 2
schemes:
- description: Base64-encoded x402 v2 exact USDC authorization on Base mainnet.
  in: header
  name: x402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/found17-com-openapi.json
  type: apiKey
- description: 'Human/business billing account identifier; pair with X-Found17-Billing-Mode: stripe.'
  in: header
  name: stripeSandboxAccount
  parameter: X-Found17-Account-Id
  sources:
  - openapi/found17-com-openapi.json
  type: apiKey
slug: found17-com-authentication
source_filename: found17-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/found17-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: Base64-encoded x402 v2 exact USDC authorization on Base mainnet.\n  sources:\n  - openapi/found17-com-openapi.json\n- name: stripeSandboxAccount\n  type: apiKey\n  in: header\n  parameter: X-Found17-Account-Id\n  description: 'Human/business billing account identifier; pair with X-Found17-Billing-Mode:\n    stripe.'\n  sources:\n  - openapi/found17-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/found17-com/authentication/found17-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Website Audit
- Product Comparison
- claim check
- public web tools
- Agents
- REST API
- MCP
- structured results
---
