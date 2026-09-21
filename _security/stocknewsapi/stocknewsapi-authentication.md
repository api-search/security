---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Stocknewsapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: StockNewsAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: StockNewsAPI
provider_slug: stocknewsapi
scheme_count: 1
schemes:
- description: API token required for all requests, passed as a query parameter
  docs: https://stocknewsapi.com/documentation
  in: query
  name: token
  type: apiKey
slug: stocknewsapi-authentication
source_filename: stocknewsapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: https://stocknewsapi.com/documentation\nschemes:\n- type: apiKey\n  name: token\n  in: query\n  description: API token required for all requests, passed as a query parameter\n  docs: https://stocknewsapi.com/documentation"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stocknewsapi/refs/heads/main/authentication/stocknewsapi-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- News
- Stocks
- Market Data
---
