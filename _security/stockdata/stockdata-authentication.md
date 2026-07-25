---
api_key_in:
- query
api_specs:
- filename: stockdata-entities-api-openapi.yml
  format: yaml
  label: StockData Entities API
  slug: stockdata-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockdata/refs/heads/main/openapi/stockdata-entities-api-openapi.yml
- filename: stockdata-news-api-openapi.yml
  format: yaml
  label: StockData News API
  slug: stockdata-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockdata/refs/heads/main/openapi/stockdata-news-api-openapi.yml
- filename: stockdata-stock-data-api-openapi.yml
  format: yaml
  label: StockData Stock Data API
  slug: stockdata-stock-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockdata/refs/heads/main/openapi/stockdata-stock-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Stockdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: StockData secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StockData
provider_slug: stockdata
scheme_count: 1
schemes:
- description: API token obtained from the StockData account dashboard after free self-serve signup (no billing details required). Added as a GET query parameter on every endpoint; an invalid or missing token returns 401 invalid_api_token.
  in: query
  name: ApiToken
  parameter: api_token
  signup: https://www.stockdata.org/register
  sources:
  - openapi/stockdata-openapi.yml
  type: apiKey
slug: stockdata-authentication
source_filename: stockdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/stockdata-openapi.yml\ndocs: https://www.stockdata.org/documentation#authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: >-\n    API token obtained from the StockData account dashboard after free self-serve signup\n    (no billing details required). Added as a GET query parameter on every endpoint;\n    an invalid or missing token returns 401 invalid_api_token.\n  signup: https://www.stockdata.org/register\n  sources:\n  - openapi/stockdata-openapi.yml\nnotes:\n  - No OAuth 2.0, OpenID Connect, or header-based auth is offered; the api_token query parameter is the only mechanism.\n  - Because the token travels in the query string, avoid logging full request URLs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockdata/refs/heads/main/authentication/stockdata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Financial Data
- Stock Market
- Market Data
- News
- Sentiment Analysis
---
