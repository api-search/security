---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gorila Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gorila secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gorila
provider_slug: gorila
scheme_count: 1
schemes:
- description: 'Static API key sent verbatim in the Authorization header, e.g. Authorization: c1deeef8-4812-4bd3-903e-8adeaff3903d'
  in: header
  name: apiKey
  parameter_name: Authorization
  sources:
  - https://gorila.com.br/core/en/docs/quickstart/
  type: apiKey
slug: gorila-authentication
source_filename: gorila-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://gorila.com.br/core/en/docs/quickstart/\ndocs: https://gorila.com.br/core/en/docs/quickstart/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nnotes: >-\n  GorilaCORE authenticates every request with a static API key passed directly\n  in the HTTP Authorization header (no \"Bearer\" prefix). Keys are issued per\n  integrating institution. No OAuth2, OpenID Connect, or mutualTLS scheme is\n  documented on the public developer surface.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  description: >-\n    Static API key sent verbatim in the Authorization header, e.g.\n    Authorization: c1deeef8-4812-4bd3-903e-8adeaff3903d\n  sources: [https://gorila.com.br/core/en/docs/quickstart/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gorila/refs/heads/main/authentication/gorila-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Investments
- Portfolio Management
- Wealth Management
- Financial Data
- Investment Consolidation
- Brazil
- API
---
