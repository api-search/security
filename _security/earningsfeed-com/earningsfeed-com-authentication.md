---
anonymous_access: false
api_key_in: []
api_specs:
- filename: earningsfeed-com-account-api-openapi.yml
  format: yaml
  label: Earnings Feed Account API
  slug: earningsfeed-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-account-api-openapi.yml
- filename: earningsfeed-com-companies-api-openapi.yml
  format: yaml
  label: Earnings Feed Companies API
  slug: earningsfeed-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-companies-api-openapi.yml
- filename: earningsfeed-com-filings-api-openapi.yml
  format: yaml
  label: Earnings Feed Filings API
  slug: earningsfeed-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-filings-api-openapi.yml
- filename: earningsfeed-com-insider-api-openapi.yml
  format: yaml
  label: Earnings Feed Insider API
  slug: earningsfeed-com-insider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-insider-api-openapi.yml
- filename: earningsfeed-com-institutional-api-openapi.yml
  format: yaml
  label: Earnings Feed Institutional API
  slug: earningsfeed-com-institutional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-institutional-api-openapi.yml
- filename: earningsfeed-com-webhooks-api-openapi.yml
  format: yaml
  label: Earnings Feed Webhooks API
  slug: earningsfeed-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Earningsfeed Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Earnings Feed secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Earnings Feed
provider_slug: earningsfeed-com
scheme_count: 1
schemes:
- description: API key sent as Bearer token in Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/earningsfeed-com-openapi.json
  type: http
slug: earningsfeed-com-authentication
source_filename: earningsfeed-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/earningsfeed-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key sent as Bearer token in Authorization header.\n  sources:\n  - openapi/earningsfeed-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/earningsfeed-com/authentication/earningsfeed-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- SEC
- Filings
- Data
---
