---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: loyalspark-online-billing-api-openapi.yml
  format: yaml
  label: Loyal Spark Billing API
  slug: loyalspark-online-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-billing-api-openapi.yml
- filename: loyalspark-online-identity-api-openapi.yml
  format: yaml
  label: Loyal Spark Identity API
  slug: loyalspark-online-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-identity-api-openapi.yml
- filename: loyalspark-online-merchant-mcp-api-openapi.yml
  format: yaml
  label: Loyal Spark Merchant MCP API
  slug: loyalspark-online-merchant-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-merchant-mcp-api-openapi.yml
- filename: loyalspark-online-merchant-rest-api-openapi.yml
  format: yaml
  label: Loyal Spark Merchant REST API
  slug: loyalspark-online-merchant-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-merchant-rest-api-openapi.yml
- filename: loyalspark-online-recipient-mcp-api-openapi.yml
  format: yaml
  label: Loyal Spark Recipient MCP API
  slug: loyalspark-online-recipient-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-recipient-mcp-api-openapi.yml
- filename: loyalspark-online-recipient-rest-api-openapi.yml
  format: yaml
  label: Loyal Spark Recipient REST API
  slug: loyalspark-online-recipient-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loyalspark-online/openapi/loyalspark-online-recipient-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Loyal Spark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loyal Spark secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Loyal Spark
provider_slug: loyalspark-online
scheme_count: 2
schemes:
- description: Agent API key (lsk_... merchant or rwk_... recipient)
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/loyalspark-online-openapi.json
  type: apiKey
- description: SIWE proof (identity-only routes)
  in: header
  name: siwx
  parameter: SIGN-IN-WITH-X
  sources:
  - openapi/loyalspark-online-openapi.json
  type: apiKey
slug: loyalspark-online-authentication
source_filename: loyalspark-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/loyalspark-online-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Agent API key (lsk_... merchant or rwk_... recipient)\n  sources:\n  - openapi/loyalspark-online-openapi.json\n- name: siwx\n  type: apiKey\n  in: header\n  parameter: SIGN-IN-WITH-X\n  description: SIWE proof (identity-only routes)\n  sources:\n  - openapi/loyalspark-online-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/loyalspark-online/authentication/loyalspark-online-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Loyalty
- Blockchain
- Rewards
- Artificial Intelligence
- Payments
---
