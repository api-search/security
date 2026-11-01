---
anonymous_access: false
api_key_in: []
api_specs:
- filename: finedata-ai-api-keys-api-openapi.yml
  format: yaml
  label: finedata-ai API Keys API
  slug: finedata-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-api-keys-api-openapi.yml
- filename: finedata-ai-async-scraping-api-openapi.yml
  format: yaml
  label: finedata-ai Async Scraping API
  slug: finedata-ai-async-scraping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-async-scraping-api-openapi.yml
- filename: finedata-ai-google-serp-api-openapi.yml
  format: yaml
  label: finedata-ai Google SERP API
  slug: finedata-ai-google-serp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-google-serp-api-openapi.yml
- filename: finedata-ai-oauth-api-openapi.yml
  format: yaml
  label: finedata-ai OAuth API
  slug: finedata-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-oauth-api-openapi.yml
- filename: finedata-ai-plans-api-openapi.yml
  format: yaml
  label: finedata-ai Plans API
  slug: finedata-ai-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-plans-api-openapi.yml
- filename: finedata-ai-proxy-profiles-byop-api-openapi.yml
  format: yaml
  label: finedata-ai Proxy Profiles (BYOP) API
  slug: finedata-ai-proxy-profiles-byop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-proxy-profiles-byop-api-openapi.yml
- filename: finedata-ai-user-api-openapi.yml
  format: yaml
  label: finedata-ai User API
  slug: finedata-ai-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-user-api-openapi.yml
- filename: finedata-ai-user-statistics-api-openapi.yml
  format: yaml
  label: finedata-ai User Statistics API
  slug: finedata-ai-user-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-user-statistics-api-openapi.yml
- filename: finedata-ai-web-scraping-api-openapi.yml
  format: yaml
  label: finedata-ai Web Scraping API
  slug: finedata-ai-web-scraping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-web-scraping-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Finedata Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: finedata-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: finedata-ai
provider_slug: finedata-ai
scheme_count: 2
schemes:
- description: API Key (recommended)
  in: header
  name: x-api-key
  type: apiKey
- bearerFormat: JWT
  description: JWT Bearer Token
  scheme: bearer
  type: http
slug: finedata-ai-authentication
source_filename: finedata-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://finedata.ai/docs/\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API Key (recommended)\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: JWT Bearer Token"
source_yaml_url: https://artifacts.apis.io/finedata-ai/authentication/finedata-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- WebScraping
- DataExtraction
- MCP
- LLM
---
