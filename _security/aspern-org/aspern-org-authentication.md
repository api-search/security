---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aspern-org-account-api-openapi.yml
  format: yaml
  label: ASPERN Account API
  slug: aspern-org-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-account-api-openapi.yml
- filename: aspern-org-agents-api-openapi.yml
  format: yaml
  label: ASPERN Agents API
  slug: aspern-org-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-agents-api-openapi.yml
- filename: aspern-org-alerts-api-openapi.yml
  format: yaml
  label: ASPERN Alerts API
  slug: aspern-org-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-alerts-api-openapi.yml
- filename: aspern-org-attestation-api-openapi.yml
  format: yaml
  label: ASPERN Attestation API
  slug: aspern-org-attestation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-attestation-api-openapi.yml
- filename: aspern-org-capital-api-openapi.yml
  format: yaml
  label: ASPERN Capital API
  slug: aspern-org-capital-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-capital-api-openapi.yml
- filename: aspern-org-commerce-api-openapi.yml
  format: yaml
  label: ASPERN Commerce API
  slug: aspern-org-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-commerce-api-openapi.yml
- filename: aspern-org-crowding-api-openapi.yml
  format: yaml
  label: ASPERN Crowding API
  slug: aspern-org-crowding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-crowding-api-openapi.yml
- filename: aspern-org-history-api-openapi.yml
  format: yaml
  label: ASPERN History API
  slug: aspern-org-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-history-api-openapi.yml
- filename: aspern-org-judgement-api-openapi.yml
  format: yaml
  label: ASPERN Judgement API
  slug: aspern-org-judgement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-judgement-api-openapi.yml
- filename: aspern-org-market-api-openapi.yml
  format: yaml
  label: ASPERN Market API
  slug: aspern-org-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-market-api-openapi.yml
- filename: aspern-org-ratings-api-openapi.yml
  format: yaml
  label: ASPERN Ratings API
  slug: aspern-org-ratings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-ratings-api-openapi.yml
- filename: aspern-org-record-api-openapi.yml
  format: yaml
  label: ASPERN Record API
  slug: aspern-org-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-record-api-openapi.yml
- filename: aspern-org-reference-api-openapi.yml
  format: yaml
  label: ASPERN Reference API
  slug: aspern-org-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-reference-api-openapi.yml
- filename: aspern-org-risk-api-openapi.yml
  format: yaml
  label: ASPERN Risk API
  slug: aspern-org-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-risk-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Aspern Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: ASPERN secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ASPERN
provider_slug: aspern-org
scheme_count: 2
schemes:
- description: Issued from the account page.
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/aspern-org-openapi.json
  type: apiKey
- description: 'Settle in-request: `<chain>:<txHash>` for a transfer already sent. Read on chain during the call and credited immediately.'
  in: header
  name: payment
  parameter: X-PAYMENT
  sources:
  - openapi/aspern-org-openapi.json
  type: apiKey
slug: aspern-org-authentication
source_filename: aspern-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/aspern-org-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Issued from the account page.\n  sources:\n  - openapi/aspern-org-openapi.json\n- name: payment\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: 'Settle in-request: `<chain>:<txHash>` for a transfer already sent. Read on chain\n    during the call and credited immediately.'\n  sources:\n  - openapi/aspern-org-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aspern-org/authentication/aspern-org-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Finance
- Blockchain
- Artificial Intelligence
- Data
- Intelligence
---
