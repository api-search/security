---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: kokofinance-net-billing-api-openapi.yml
  format: yaml
  label: kokofinance-net Billing API
  slug: kokofinance-net-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-billing-api-openapi.yml
- filename: kokofinance-net-cards-api-openapi.yml
  format: yaml
  label: kokofinance-net Cards API
  slug: kokofinance-net-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-cards-api-openapi.yml
- filename: kokofinance-net-developers-api-openapi.yml
  format: yaml
  label: kokofinance-net Developers API
  slug: kokofinance-net-developers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-developers-api-openapi.yml
- filename: kokofinance-net-intelligence-api-openapi.yml
  format: yaml
  label: kokofinance-net Intelligence API
  slug: kokofinance-net-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-intelligence-api-openapi.yml
- filename: kokofinance-net-international-api-openapi.yml
  format: yaml
  label: kokofinance-net International API
  slug: kokofinance-net-international-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-international-api-openapi.yml
- filename: kokofinance-net-platform-api-openapi.yml
  format: yaml
  label: kokofinance-net Platform API
  slug: kokofinance-net-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-platform-api-openapi.yml
- filename: kokofinance-net-portfolio-api-openapi.yml
  format: yaml
  label: kokofinance-net Portfolio API
  slug: kokofinance-net-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-portfolio-api-openapi.yml
- filename: kokofinance-net-reference-api-openapi.yml
  format: yaml
  label: kokofinance-net Reference API
  slug: kokofinance-net-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-reference-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kokofinance Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: kokofinance-net secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: kokofinance-net
provider_slug: kokofinance-net
scheme_count: 1
schemes:
- description: 'Your Koko API key (format: koko_xxxxx)'
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/kokofinance-net-openapi.json
  type: apiKey
slug: kokofinance-net-authentication
source_filename: kokofinance-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/kokofinance-net-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Your Koko API key (format: koko_xxxxx)'\n  sources:\n  - openapi/kokofinance-net-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kokofinance-net/authentication/kokofinance-net-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Credit-Card
- API
- MCP
---
