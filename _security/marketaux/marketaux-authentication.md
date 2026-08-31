---
api_key_in:
- query
api_specs:
- filename: marketaux-entities-api-openapi.yml
  format: yaml
  label: MarketAux Entities API
  slug: marketaux-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketaux/refs/heads/main/openapi/marketaux-entities-api-openapi.yml
- filename: marketaux-news-api-openapi.yml
  format: yaml
  label: MarketAux News API
  slug: marketaux-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketaux/refs/heads/main/openapi/marketaux-news-api-openapi.yml
- filename: marketaux-sources-api-openapi.yml
  format: yaml
  label: MarketAux Sources API
  slug: marketaux-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketaux/refs/heads/main/openapi/marketaux-sources-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Marketaux Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarketAux secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MarketAux
provider_slug: marketaux
scheme_count: 1
schemes:
- description: Your API token, found on your account dashboard after signing up at https://www.marketaux.com/register. Passed as a GET parameter on every request.
  in: query
  name: apiToken
  parameter: api_token
  sources:
  - openapi/marketaux-openapi.yml
  type: apiKey
slug: marketaux-authentication
source_filename: marketaux-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/marketaux-openapi.yml\ndocs: https://www.marketaux.com/documentation#authentication\nnotes: >-\n  The documentation's Authentication section confirms the single auth\n  mechanism: sign up free, find the API token on the account dashboard, and\n  add it to any endpoint as the api_token GET parameter. No OAuth, no header\n  schemes.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: Your API token, found on your account dashboard after signing up at https://www.marketaux.com/register.\n    Passed as a GET parameter on every request.\n  sources:\n  - openapi/marketaux-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketaux/refs/heads/main/authentication/marketaux-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- News
- Financial News
- Stock Market
- Sentiment Analysis
- Market Data
- Entity Recognition
- Public APIs
---
