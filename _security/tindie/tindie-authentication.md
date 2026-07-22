---
api_key_in:
- query
- header
api_specs:
- filename: tindie-openapi.yml
  format: yaml
  label: Tindie API
  slug: tindie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tindie/refs/heads/main/openapi/tindie-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tindie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tindie secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tindie
provider_slug: tindie
scheme_count: 3
schemes:
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/tindie-openapi.yml
  type: apiKey
- in: query
  name: usernameQuery
  parameter: username
  sources:
  - openapi/tindie-openapi.yml
  type: apiKey
- format: ApiKey <username>:<api_key>
  in: header
  name: authorizationHeader
  parameter: Authorization
  sources:
  - openapi/tindie-openapi.yml
  type: apiKey
slug: tindie-authentication
source_filename: tindie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tindie-openapi.yml\ndocs: https://www.tindie.com/help/\nsummary:\n  types: [apiKey]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  note: >-\n    Tindie uses Django Tastypie ApiKeyAuthentication. Authenticated calls to the\n    order and orderitem resources require an API key issued from the seller's\n    account settings, passed as `api_key` + `username` query parameters or the\n    header `Authorization: ApiKey <username>:<api_key>`. The product resource is\n    public and requires no authentication. Verified live: /order/ and\n    /orderitem/ return HTTP 401 without credentials; /product/ is open.\nschemes:\n  - name: apiKeyQuery\n    type: apiKey\n    in: query\n    parameter: api_key\n    sources: [openapi/tindie-openapi.yml]\n  - name: usernameQuery\n    type: apiKey\n    in: query\n    parameter: username\n    sources: [openapi/tindie-openapi.yml]\n  - name: authorizationHeader\n    type: apiKey\n    in:\
  \ header\n    parameter: Authorization\n    format: 'ApiKey <username>:<api_key>'\n    sources: [openapi/tindie-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tindie/refs/heads/main/authentication/tindie-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Marketplace
- Hardware
- Electronics
- Maker
- eCommerce
- Open Source Hardware
- Orders
---
