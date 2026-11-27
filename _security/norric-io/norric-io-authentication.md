---
anonymous_access: false
api_key_in: []
api_specs:
- filename: norric-io-health-api-openapi.yml
  format: yaml
  label: Norric Health API
  slug: norric-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-health-api-openapi.yml
- filename: norric-io-intelligence-rest-api-openapi.yml
  format: yaml
  label: Norric Intelligence REST API
  slug: norric-io-intelligence-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-intelligence-rest-api-openapi.yml
- filename: norric-io-mcp-api-openapi.yml
  format: yaml
  label: Norric MCP API
  slug: norric-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-mcp-api-openapi.yml
- filename: norric-io-paid-danish-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Danish company intelligence API
  slug: norric-io-paid-danish-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-danish-company-intelligence-api-openapi.yml
- filename: norric-io-paid-estonian-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Estonian company intelligence API
  slug: norric-io-paid-estonian-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-estonian-company-intelligence-api-openapi.yml
- filename: norric-io-paid-finnish-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Finnish company intelligence API
  slug: norric-io-paid-finnish-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-finnish-company-intelligence-api-openapi.yml
- filename: norric-io-paid-french-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid French company intelligence API
  slug: norric-io-paid-french-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-french-company-intelligence-api-openapi.yml
- filename: norric-io-paid-norwegian-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Norwegian company intelligence API
  slug: norric-io-paid-norwegian-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-norwegian-company-intelligence-api-openapi.yml
- filename: norric-io-paid-swedish-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Swedish company intelligence API
  slug: norric-io-paid-swedish-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-swedish-company-intelligence-api-openapi.yml
- filename: norric-io-service-api-openapi.yml
  format: yaml
  label: Norric Service API
  slug: norric-io-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-service-api-openapi.yml
auth_types: []
description: Authentication schemes for Norric API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Norric Authentication
name_suffix: Authentication
oauth_flows: []
overview: Norric declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Norric
provider_slug: norric-io
scheme_count: 1
schemes:
- evidence: paid calls use x402 on Base Sepolia testnet.
  header: x402
  how_to_obtain: Request access by email to edgar@norric.io.
  location: header
  name: x402
  type: apiKey
slug: norric-io-authentication
source_filename: norric-io-authentication.yml
source_heading: Authentication Profile
source_url: https://norric.io/api-keys
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://norric.io/api-keys\nsources:\n- https://norric.io/api-keys\ndescription: Authentication schemes for Norric API\nschemes:\n- type: apiKey\n  name: x402\n  evidence: paid calls use x402 on Base Sepolia testnet.\n  location: header\n  header: x402\n  how_to_obtain: Request access by email to edgar@norric.io.\ndocs: https://norric.io/api-keys\n"
source_yaml_url: https://artifacts.apis.io/norric-io/authentication/norric-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- EU
- Artificial Intelligence
- Registers
---
