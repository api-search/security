---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nomior-com-alternative-data-api-openapi.yml
  format: yaml
  label: Nomior Alternative data API
  slug: nomior-com-alternative-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-alternative-data-api-openapi.yml
- filename: nomior-com-companies-api-openapi.yml
  format: yaml
  label: Nomior Companies API
  slug: nomior-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-companies-api-openapi.yml
- filename: nomior-com-filings-api-openapi.yml
  format: yaml
  label: Nomior Filings API
  slug: nomior-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-filings-api-openapi.yml
- filename: nomior-com-financials-api-openapi.yml
  format: yaml
  label: Nomior Financials API
  slug: nomior-com-financials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-financials-api-openapi.yml
- filename: nomior-com-government-api-openapi.yml
  format: yaml
  label: Nomior Government API
  slug: nomior-com-government-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-government-api-openapi.yml
- filename: nomior-com-insider-api-openapi.yml
  format: yaml
  label: Nomior Insider API
  slug: nomior-com-insider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-insider-api-openapi.yml
- filename: nomior-com-news-api-openapi.yml
  format: yaml
  label: Nomior News API
  slug: nomior-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-news-api-openapi.yml
- filename: nomior-com-people-api-openapi.yml
  format: yaml
  label: Nomior People API
  slug: nomior-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-people-api-openapi.yml
- filename: nomior-com-portfolios-api-openapi.yml
  format: yaml
  label: Nomior Portfolios API
  slug: nomior-com-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-portfolios-api-openapi.yml
- filename: nomior-com-reference-api-openapi.yml
  format: yaml
  label: Nomior Reference API
  slug: nomior-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-reference-api-openapi.yml
- filename: nomior-com-scores-api-openapi.yml
  format: yaml
  label: Nomior Scores API
  slug: nomior-com-scores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-scores-api-openapi.yml
- filename: nomior-com-screener-api-openapi.yml
  format: yaml
  label: Nomior Screener API
  slug: nomior-com-screener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-screener-api-openapi.yml
- filename: nomior-com-tokens-api-openapi.yml
  format: yaml
  label: Nomior Tokens API
  slug: nomior-com-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomior-com/openapi/nomior-com-tokens-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Nomior Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nomior secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nomior
provider_slug: nomior-com
scheme_count: 2
schemes:
- description: 'API key as a bearer token: "Authorization: Bearer nmr_live_…".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/invest-openapi.json
  type: http
- description: API key header alternative to the Authorization bearer scheme.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/invest-openapi.json
  type: apiKey
slug: nomior-com-authentication
source_filename: nomior-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/invest-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key as a bearer token: \"Authorization: Bearer nmr_live_…\".'\n  sources:\n  - openapi/invest-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key header alternative to the Authorization bearer scheme.\n  sources:\n  - openapi/invest-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nomior-com/authentication/nomior-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Data
- Finance
- Knowledge
---
