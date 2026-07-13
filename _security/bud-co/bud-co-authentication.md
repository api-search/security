---
api_key_in: []
api_specs:
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Connect API
  slug: bud-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud First-Party Ingestion API
  slug: bud-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Customers Platform API
  slug: bud-customers-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Financial Data API
  slug: bud-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Enrichment API
  slug: bud-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Financial Insights API
  slug: bud-financial-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Intelligent Search API
  slug: bud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Affordability and Assess API
  slug: bud-affordability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Customer Characteristics API
  slug: bud-characteristics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Goals and Budgets API
  slug: bud-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Payments API
  slug: bud-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Embedded Widgets API
  slug: bud-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bud Co Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bud Financial secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bud Financial
provider_slug: bud-co
scheme_count: 2
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/bud-platform-openapi.yml
  type: http
- description: 'Authentication flow:


    1. Perform OAuth2 Client Credentials authentication using API Credentials (`client_id`,`client_secret`) to obtain an `access_token` against `/v1/oauth/token` endpoint,

    2. Use `access_token` as Bearer Authorisation for every other API request,

    3. Include `X-Client-Id` (=client_id) within the header of every API request,

    4. Note that some of the requests may also require `X-Cus'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /v1/oauth/token
  name: OAuth2
  sources:
  - openapi/bud-platform-openapi.yml
  type: oauth2
slug: bud-co-authentication
source_filename: bud-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bud-platform-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/bud-platform-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth/token\n    scopes: 0\n  description: |-\n    Authentication flow:\n\n    1. Perform OAuth2 Client Credentials authentication using API Credentials (`client_id`,`client_secret`) to obtain an `access_token` against `/v1/oauth/token` endpoint,\n    2. Use `access_token` as Bearer Authorisation for every other API request,\n    3. Include `X-Client-Id` (=client_id) within the header of every API request,\n    4. Note that some of the requests may also require `X-Cus\n  sources:\n  - openapi/bud-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/authentication/bud-co-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Open Banking
- Transaction Enrichment
- Categorization
- Affordability
- Payments
- AISP
- PISP
- Financial Data
- FinTech
- UK
- AI
- Machine Learning
---
