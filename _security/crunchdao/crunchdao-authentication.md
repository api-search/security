---
api_key_in:
- query
api_specs:
- filename: crunchdao-tournament-openapi.json
  format: json
  label: CrunchDAO Tournament API
  slug: crunchdao-tournament-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchdao/refs/heads/main/openapi/crunchdao-tournament-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Crunchdao Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrunchDAO secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CrunchDAO
provider_slug: crunchdao
scheme_count: 2
schemes:
- in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/crunchdao-tournament-openapi.json
  type: apiKey
- name: accessToken
  scheme: Bearer
  sources:
  - openapi/crunchdao-tournament-openapi.json
  type: http
slug: crunchdao-authentication
source_filename: crunchdao-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/crunchdao-tournament-openapi.json\ndocs: https://docs.crunchdao.com/technical/tournament-api\nkey_management: https://hub.crunchdao.com/account/api\nnotes: 'Two token types accepted. API Key: header `Authorization: API-Key <token>`\n  or `?apiKey=<token>`. Access Token: header `Authorization: Bearer <token>` or\n  `?accessToken=<token>`. The crunch-cli reads the API key from the CRUNCH_API_KEY\n  environment variable.'\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/crunchdao-tournament-openapi.json\n- name: accessToken\n  type: http\n  scheme: Bearer\n  sources:\n  - openapi/crunchdao-tournament-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchdao/refs/heads/main/authentication/crunchdao-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Crypto Web3
- Machine Learning
- Data Science
- Competitions
- Collective Intelligence
- Quantitative Finance
- Predictions
---
