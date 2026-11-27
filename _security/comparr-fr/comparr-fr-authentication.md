---
anonymous_access: true
api_key_in: []
api_specs:
- filename: comparr-fr-comparatifs-api-openapi.yml
  format: yaml
  label: Comparr Comparatifs API
  slug: comparr-fr-comparatifs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparr-fr/openapi/comparr-fr-comparatifs-api-openapi.yml
- filename: comparr-fr-deals-api-openapi.yml
  format: yaml
  label: Comparr Deals API
  slug: comparr-fr-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparr-fr/openapi/comparr-fr-deals-api-openapi.yml
- filename: comparr-fr-discovery-api-openapi.yml
  format: yaml
  label: Comparr Discovery API
  slug: comparr-fr-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparr-fr/openapi/comparr-fr-discovery-api-openapi.yml
- filename: comparr-fr-products-api-openapi.yml
  format: yaml
  label: Comparr Products API
  slug: comparr-fr-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparr-fr/openapi/comparr-fr-products-api-openapi.yml
- filename: comparr-fr-searches-api-openapi.yml
  format: yaml
  label: Comparr Searches API
  slug: comparr-fr-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparr-fr/openapi/comparr-fr-searches-api-openapi.yml
- filename: comparr-fr-versus-api-openapi.yml
  format: yaml
  label: Comparr Versus API
  slug: comparr-fr-versus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparr-fr/openapi/comparr-fr-versus-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Comparr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comparr declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Comparr
provider_slug: comparr-fr
scheme_count: 2
schemes:
- applies_to: REST API https://www.comparr.fr/api/v1
  description: Unauthenticated public access.
  evidence: 'Lecture du catalogue : publique, sans clé API.'
  name: anonymous
  type: none
- applies_to: MCP https://www.comparr.fr/mcp
  description: Remote MCP server with no authentication.
  evidence: 'Transport : Streamable HTTP, sans état. Authentification : aucune.'
  name: anonymous-mcp
  type: none
slug: comparr-fr-authentication
source_filename: comparr-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.comparr.fr/api/docs\ndocs: https://www.comparr.fr/api/docs\nsummary: The Comparr API and MCP server are public and require no API key, account or token. The OpenAPI contract declares no securitySchemes. Quotas are keyed on client IP and User-Agent instead of a credential.\nschemes:\n- type: none\n  name: anonymous\n  description: Unauthenticated public access.\n  evidence: \"Lecture du catalogue : publique, sans clé API.\"\n  applies_to: REST API https://www.comparr.fr/api/v1\n- type: none\n  name: anonymous-mcp\n  description: Remote MCP server with no authentication.\n  evidence: \"Transport : Streamable HTTP, sans état. Authentification : aucune.\"\n  applies_to: MCP https://www.comparr.fr/mcp\n"
source_yaml_url: https://artifacts.apis.io/comparr-fr/authentication/comparr-fr-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Price Comparison
- E-Commerce
- Shopping
- Artificial Intelligence
- Product Reviews
- AI Agents
- MCP
- France
---
