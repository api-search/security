---
anonymous_access: false
api_key_in: []
api_specs:
- filename: evidinvest-com-calculations-api-openapi.yml
  format: yaml
  label: evidinvest-com Calculations API
  slug: evidinvest-com-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-calculations-api-openapi.yml
- filename: evidinvest-com-financial-data-api-openapi.yml
  format: yaml
  label: evidinvest-com Financial Data API
  slug: evidinvest-com-financial-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-financial-data-api-openapi.yml
- filename: evidinvest-com-machine-payments-api-openapi.yml
  format: yaml
  label: evidinvest-com Machine Payments API
  slug: evidinvest-com-machine-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-machine-payments-api-openapi.yml
- filename: evidinvest-com-market-data-api-openapi.yml
  format: yaml
  label: evidinvest-com Market Data API
  slug: evidinvest-com-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-market-data-api-openapi.yml
- filename: evidinvest-com-portfolio-api-openapi.yml
  format: yaml
  label: evidinvest-com Portfolio API
  slug: evidinvest-com-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-portfolio-api-openapi.yml
- filename: evidinvest-com-sec-filings-api-openapi.yml
  format: yaml
  label: evidinvest-com SEC Filings API
  slug: evidinvest-com-sec-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-sec-filings-api-openapi.yml
- filename: evidinvest-com-user-lists-api-openapi.yml
  format: yaml
  label: evidinvest-com User Lists API
  slug: evidinvest-com-user-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-user-lists-api-openapi.yml
- filename: evidinvest-com-valuation-api-openapi.yml
  format: yaml
  label: evidinvest-com Valuation API
  slug: evidinvest-com-valuation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-valuation-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Evidinvest Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: evidinvest-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: evidinvest-com
provider_slug: evidinvest-com
scheme_count: 1
schemes:
- bearerFormat: EvidInvest API key (evid_sk_...)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/evidinvest-com-openapi.json
  - openapi/mcp_openapi.json
  type: http
slug: evidinvest-com-authentication
source_filename: evidinvest-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/evidinvest-com-openapi.json, openapi/mcp_openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: EvidInvest API key (evid_sk_...)\n  sources:\n  - openapi/evidinvest-com-openapi.json\n  - openapi/mcp_openapi.json\n"
source_yaml_url: https://artifacts.apis.io/evidinvest-com/authentication/evidinvest-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Finance
- Valuation
- API
- Data
---
