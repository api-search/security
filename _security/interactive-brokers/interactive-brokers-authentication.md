---
api_key_in: []
api_specs:
- filename: interactive-brokers-accounts-api-openapi.yml
  format: yaml
  label: Interactive Brokers Accounts API
  slug: interactive-brokers-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-accounts-api-openapi.yml
- filename: interactive-brokers-contracts-api-openapi.yml
  format: yaml
  label: Interactive Brokers Contracts API
  slug: interactive-brokers-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-contracts-api-openapi.yml
- filename: interactive-brokers-market-data-api-openapi.yml
  format: yaml
  label: Interactive Brokers Market Data API
  slug: interactive-brokers-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-market-data-api-openapi.yml
- filename: interactive-brokers-orders-api-openapi.yml
  format: yaml
  label: Interactive Brokers Orders API
  slug: interactive-brokers-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-orders-api-openapi.yml
- filename: interactive-brokers-portfolio-api-openapi.yml
  format: yaml
  label: Interactive Brokers Portfolio API
  slug: interactive-brokers-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-portfolio-api-openapi.yml
- filename: interactive-brokers-sessions-api-openapi.yml
  format: yaml
  label: Interactive Brokers Sessions API
  slug: interactive-brokers-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-sessions-api-openapi.yml
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
