---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alpinedataworks-com-account-api-openapi.yml
  format: yaml
  label: AlpineDataWorks.AI Account API
  slug: alpinedataworks-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alpinedataworks-com/openapi/alpinedataworks-com-account-api-openapi.yml
- filename: alpinedataworks-com-billing-api-openapi.yml
  format: yaml
  label: AlpineDataWorks.AI Billing API
  slug: alpinedataworks-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alpinedataworks-com/openapi/alpinedataworks-com-billing-api-openapi.yml
- filename: alpinedataworks-com-catalog-api-openapi.yml
  format: yaml
  label: AlpineDataWorks.AI Catalog API
  slug: alpinedataworks-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alpinedataworks-com/openapi/alpinedataworks-com-catalog-api-openapi.yml
- filename: alpinedataworks-com-mcp-api-openapi.yml
  format: yaml
  label: AlpineDataWorks.AI MCP API
  slug: alpinedataworks-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alpinedataworks-com/openapi/alpinedataworks-com-mcp-api-openapi.yml
- filename: alpinedataworks-com-products-api-openapi.yml
  format: yaml
  label: AlpineDataWorks.AI Products API
  slug: alpinedataworks-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alpinedataworks-com/openapi/alpinedataworks-com-products-api-openapi.yml
- filename: alpinedataworks-com-public-api-openapi.yml
  format: yaml
  label: AlpineDataWorks.AI Public API
  slug: alpinedataworks-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alpinedataworks-com/openapi/alpinedataworks-com-public-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AlpineDataWorks.AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlpineDataWorks.AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AlpineDataWorks.AI
provider_slug: alpinedataworks-com
scheme_count: 1
schemes:
- description: 'Public demo key: adw_free_demo (Free tier). Gold/Platinum require an issued API key. Production: SHA-256 hashed keys stored in Cloudflare KV.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/alpinedataworks-com-openapi.json
  - openapi/alpinedataworks-com.json
  type: http
slug: alpinedataworks-com-authentication
source_filename: alpinedataworks-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/alpinedataworks-com-openapi.json, openapi/alpinedataworks-com.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Public demo key: adw_free_demo (Free tier). Gold/Platinum require an issued\n    API key. Production: SHA-256 hashed keys stored in Cloudflare KV.'\n  sources:\n  - openapi/alpinedataworks-com-openapi.json\n  - openapi/alpinedataworks-com.json\n"
source_yaml_url: https://artifacts.apis.io/alpinedataworks-com/authentication/alpinedataworks-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Artificial Intelligence
- Intelligence
- Analytics
- Open Data
---
