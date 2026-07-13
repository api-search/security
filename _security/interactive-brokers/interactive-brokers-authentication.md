---
api_key_in: []
api_specs:
- filename: interactive-brokers-web-api-openapi.yml
  format: yaml
  label: Interactive Brokers Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-web-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Interactive Brokers Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Interactive Brokers secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Interactive Brokers
provider_slug: interactive-brokers
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://www.interactivebrokers.com/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://www.interactivebrokers.com/token
  name: oauth2
  sources:
  - openapi/interactive-brokers-web-api-openapi.yml
  type: oauth2
slug: interactive-brokers-authentication
source_filename: interactive-brokers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/interactive-brokers-web-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.interactivebrokers.com/authorize\n    tokenUrl: https://www.interactivebrokers.com/token\n    scopes: 0\n  sources:\n  - openapi/interactive-brokers-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/authentication/interactive-brokers-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Brokerage
- Market Data
- Orders
- Portfolio
- Trading
---
