---
api_key_in:
- query
api_specs:
- filename: buxfer-openapi.yml
  format: yaml
  label: Buxfer API
  slug: buxfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buxfer/refs/heads/main/openapi/buxfer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Buxfer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buxfer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Buxfer
provider_slug: buxfer
scheme_count: 1
schemes:
- description: Ephemeral token returned by the login operation, passed as a query parameter on every subsequent request.
  in: query
  name: token
  parameter: token
  sources:
  - openapi/buxfer-openapi.yml
  type: apiKey
slug: buxfer-authentication
source_filename: buxfer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/buxfer-openapi.yml\ndocs: https://www.buxfer.com/help/api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  model: login-token\n  notes: >-\n    Buxfer does not use OAuth. A client authenticates once with the account\n    email and password via the login operation, which returns a unique ephemeral\n    token. That token is then passed as a `token` query parameter on every\n    subsequent request. There are no OAuth scopes; access is full-account.\nlogin_flow:\n  operation: login\n  request:\n    email: account email\n    password: account password\n  returns: token\n  token_param: token\n  token_lifetime: ephemeral\nschemes:\n- name: token\n  type: apiKey\n  in: query\n  parameter: token\n  description: >-\n    Ephemeral token returned by the login operation, passed as a query parameter\n    on every subsequent request.\n  sources:\n  - openapi/buxfer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buxfer/refs/heads/main/authentication/buxfer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Personal Finance
- Money Management
- Budgeting
- Banking
- Fintech
- Financial Data
- Transactions
- Investments
- Expense Tracking
---
