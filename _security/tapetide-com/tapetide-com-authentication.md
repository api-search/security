---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tapetide-com-account-api-openapi.yml
  format: yaml
  label: Tapetide Account API
  slug: tapetide-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-account-api-openapi.yml
- filename: tapetide-com-derivatives-api-openapi.yml
  format: yaml
  label: Tapetide Derivatives API
  slug: tapetide-com-derivatives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-derivatives-api-openapi.yml
- filename: tapetide-com-filings-api-openapi.yml
  format: yaml
  label: Tapetide Filings API
  slug: tapetide-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-filings-api-openapi.yml
- filename: tapetide-com-fundamentals-api-openapi.yml
  format: yaml
  label: Tapetide Fundamentals API
  slug: tapetide-com-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-fundamentals-api-openapi.yml
- filename: tapetide-com-funds-api-openapi.yml
  format: yaml
  label: Tapetide Funds API
  slug: tapetide-com-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-funds-api-openapi.yml
- filename: tapetide-com-indices-api-openapi.yml
  format: yaml
  label: Tapetide Indices API
  slug: tapetide-com-indices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-indices-api-openapi.yml
- filename: tapetide-com-ipos-api-openapi.yml
  format: yaml
  label: Tapetide Ipos API
  slug: tapetide-com-ipos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-ipos-api-openapi.yml
- filename: tapetide-com-live-api-openapi.yml
  format: yaml
  label: Tapetide Live API
  slug: tapetide-com-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-live-api-openapi.yml
- filename: tapetide-com-macro-api-openapi.yml
  format: yaml
  label: Tapetide Macro API
  slug: tapetide-com-macro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-macro-api-openapi.yml
- filename: tapetide-com-market-api-openapi.yml
  format: yaml
  label: Tapetide Market API
  slug: tapetide-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-market-api-openapi.yml
- filename: tapetide-com-news-api-openapi.yml
  format: yaml
  label: Tapetide News API
  slug: tapetide-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-news-api-openapi.yml
- filename: tapetide-com-options-api-openapi.yml
  format: yaml
  label: Tapetide Options API
  slug: tapetide-com-options-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-options-api-openapi.yml
- filename: tapetide-com-ownership-api-openapi.yml
  format: yaml
  label: Tapetide Ownership API
  slug: tapetide-com-ownership-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-ownership-api-openapi.yml
- filename: tapetide-com-prices-api-openapi.yml
  format: yaml
  label: Tapetide Prices API
  slug: tapetide-com-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-prices-api-openapi.yml
- filename: tapetide-com-reference-api-openapi.yml
  format: yaml
  label: Tapetide Reference API
  slug: tapetide-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-reference-api-openapi.yml
- filename: tapetide-com-scores-api-openapi.yml
  format: yaml
  label: Tapetide Scores API
  slug: tapetide-com-scores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-scores-api-openapi.yml
- filename: tapetide-com-screens-api-openapi.yml
  format: yaml
  label: Tapetide Screens API
  slug: tapetide-com-screens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-screens-api-openapi.yml
- filename: tapetide-com-shareholders-api-openapi.yml
  format: yaml
  label: Tapetide Shareholders API
  slug: tapetide-com-shareholders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-shareholders-api-openapi.yml
- filename: tapetide-com-stocks-api-openapi.yml
  format: yaml
  label: Tapetide Stocks API
  slug: tapetide-com-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapetide-com/openapi/tapetide-com-stocks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tapetide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tapetide secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tapetide
provider_slug: tapetide-com
scheme_count: 1
schemes:
- description: Tapetide personal token (tpt_rt_...) or access token (tpt....).
  name: bearer
  scheme: bearer
  sources:
  - openapi/tapetide-com-openapi.json
  type: http
slug: tapetide-com-authentication
source_filename: tapetide-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/tapetide-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Tapetide personal token (tpt_rt_...) or access token (tpt....).\n  sources:\n  - openapi/tapetide-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tapetide-com/authentication/tapetide-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Finance
- Stock-Market
- Analytics
- Indian-Market
---
