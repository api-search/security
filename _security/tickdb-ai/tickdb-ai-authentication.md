---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tickdb-ai-account-api-openapi.yml
  format: yaml
  label: tickdb-ai Account API
  slug: tickdb-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-account-api-openapi.yml
- filename: tickdb-ai-fundamentals-capital-actions-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Capital Actions API
  slug: tickdb-ai-fundamentals-capital-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-capital-actions-api-openapi.yml
- filename: tickdb-ai-fundamentals-company-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Company API
  slug: tickdb-ai-fundamentals-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-company-api-openapi.yml
- filename: tickdb-ai-fundamentals-events-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Events API
  slug: tickdb-ai-fundamentals-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-events-api-openapi.yml
- filename: tickdb-ai-fundamentals-financials-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Financials API
  slug: tickdb-ai-fundamentals-financials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-financials-api-openapi.yml
- filename: tickdb-ai-fundamentals-holders-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Holders API
  slug: tickdb-ai-fundamentals-holders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-holders-api-openapi.yml
- filename: tickdb-ai-fundamentals-valuation-industry-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Valuation Industry API
  slug: tickdb-ai-fundamentals-valuation-industry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-valuation-industry-api-openapi.yml
- filename: tickdb-ai-market-api-openapi.yml
  format: yaml
  label: tickdb-ai Market API
  slug: tickdb-ai-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-market-api-openapi.yml
- filename: tickdb-ai-symbols-api-openapi.yml
  format: yaml
  label: tickdb-ai Symbols API
  slug: tickdb-ai-symbols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-symbols-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tickdb Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: tickdb-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: tickdb-ai
provider_slug: tickdb-ai
scheme_count: 1
schemes:
- description: API key authentication via X-API-Key header
  docs:
  - note: Shows X-API-Key header usage
    url: https://docs.tickdb.ai/zh-Hans/quick-start
  in: header
  name: X-API-Key
  type: apiKey
slug: tickdb-ai-authentication
source_filename: tickdb-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/tickdb-ai-openapi.yml\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key authentication via X-API-Key header\n    docs:\n      - url: https://docs.tickdb.ai/zh-Hans/quick-start\n        note: Shows X-API-Key header usage\n"
source_yaml_url: https://artifacts.apis.io/tickdb-ai/authentication/tickdb-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Market-Data
- Real-time
- API
---
