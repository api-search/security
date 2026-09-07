---
anonymous_access: false
api_key_in:
- query
- header
api_specs:
- filename: amazon-scraper-api-openapi-original.json
  format: json
  label: Amazon Scraper REST API
  slug: amazon-scraper-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-scraper-api/refs/heads/main/openapi/amazon-scraper-api-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Amazon Scraper Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Scraper API secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Amazon Scraper API
provider_slug: amazon-scraper-api
scheme_count: 3
schemes:
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/amazon-scraper-api-openapi-original.json
  - https://amazonscraperapi.com/docs/guides/authentication
  type: apiKey
- in: header
  name: apiKeyHeader
  note: Documented in the provider's ai-plugin.json and published Claude Skills; not declared in the OpenAPI securitySchemes.
  parameter: X-API-Key
  sources:
  - well-known/amazon-scraper-api-ai-plugin.json
  - skills/amazon-scraper-api-scrape-amazon-product.md
  type: apiKey
- name: bearerAuth
  note: Authorization Bearer with the same API key, per ai-plugin.json and the OpenAPI.
  scheme: bearer
  sources:
  - openapi/amazon-scraper-api-openapi-original.json
  type: http
slug: amazon-scraper-api-authentication
source_filename: amazon-scraper-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/amazon-scraper-api-openapi-original.json\ndocs: https://amazonscraperapi.com/docs/guides/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\n  - header\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/amazon-scraper-api-openapi-original.json\n  - https://amazonscraperapi.com/docs/guides/authentication\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  note: Documented in the provider's ai-plugin.json and published Claude Skills; not declared in the OpenAPI securitySchemes.\n  sources:\n  - well-known/amazon-scraper-api-ai-plugin.json\n  - skills/amazon-scraper-api-scrape-amazon-product.md\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  note: Authorization Bearer with the same API key, per ai-plugin.json and the OpenAPI.\n  sources:\n  - openapi/amazon-scraper-api-openapi-original.json\nkey_format:\n\
  \  prefixes:\n  - prefix: asa_live_\n    meaning: Production traffic\n  - prefix: asa_test_\n    meaning: Sandbox keys (roadmap only - not yet live; would return deterministic fixtures and never bill)\n  shortprefix: 12 characters after the prefix identify a key in the dashboard and logs without revealing the secret\nmanagement:\n  console: https://app.amazonscraperapi.com\n  max_active_keys_per_workspace: 20\n  rotation: Generate a second key, deploy, revoke the old one; revocation is global within ~30 seconds and revoked keys return 401 {\"error\":\"revoked\"}\n  usage_retention_after_revoke: 90 days\nnotes:\n- Unauthorized (401) requests are never billed.\n- Keys are workspace-scoped; the monthly credit allowance is per workspace, not per key.\n- IP allow-lists are on the roadmap for Pro and Custom plans.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-scraper-api/refs/heads/main/authentication/amazon-scraper-api-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Web Scraping
- Data Extraction
- E-Commerce Data
- Amazon
- marketplace data
- Product Intelligence
- Price Monitoring
- Competitor Research
- MCP
- Agent Tooling
---
