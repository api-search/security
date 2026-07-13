---
api_key_in: []
api_specs:
- filename: tink-oauth-api-openapi.yml
  format: yaml
  label: Tink OAuth API
  slug: tink-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-oauth-api-openapi.yml
- filename: tink-account-check-api-openapi.yml
  format: yaml
  label: Tink Account Check API
  slug: tink-account-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-account-check-api-openapi.yml
- filename: tink-data-api-openapi.yml
  format: yaml
  label: Tink Data API
  slug: tink-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-data-api-openapi.yml
- filename: tink-data-enrichment-api-openapi.yml
  format: yaml
  label: Tink Data Enrichment API
  slug: tink-data-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-data-enrichment-api-openapi.yml
- filename: tink-payments-api-openapi.yml
  format: yaml
  label: Tink Payments API
  slug: tink-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-payments-api-openapi.yml
- filename: tink-risk-reports-api-openapi.yml
  format: yaml
  label: Tink Risk and Reports API
  slug: tink-risk-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-risk-reports-api-openapi.yml
- filename: tink-money-manager-api-openapi.yml
  format: yaml
  label: Tink Money Manager API
  slug: tink-money-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-money-manager-api-openapi.yml
- filename: tink-connector-api-openapi.yml
  format: yaml
  label: Tink Connector API
  slug: tink-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-connector-api-openapi.yml
- filename: tink-webhooks-api-openapi.yml
  format: yaml
  label: Tink Webhooks API
  slug: tink-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tink Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tink secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tink
provider_slug: tink-com
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tink-account-check-api-openapi.yml
  - openapi/tink-connector-api-openapi.yml
  - openapi/tink-data-api-openapi.yml
  - openapi/tink-data-enrichment-api-openapi.yml
  - openapi/tink-money-manager-api-openapi.yml
  - openapi/tink-oauth-api-openapi.yml
  - openapi/tink-payments-api-openapi.yml
  - openapi/tink-risk-reports-api-openapi.yml
  - openapi/tink-webhooks-api-openapi.yml
  type: http
slug: tink-com-authentication
source_filename: tink-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tink-account-check-api-openapi.yml, openapi/tink-connector-api-openapi.yml,\n  openapi/tink-data-api-openapi.yml, openapi/tink-data-enrichment-api-openapi.yml, openapi/tink-money-manager-api-openapi.yml,\n  openapi/tink-oauth-api-openapi.yml, openapi/tink-payments-api-openapi.yml, openapi/tink-risk-reports-api-openapi.yml,\n  openapi/tink-webhooks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tink-account-check-api-openapi.yml\n  - openapi/tink-connector-api-openapi.yml\n  - openapi/tink-data-api-openapi.yml\n  - openapi/tink-data-enrichment-api-openapi.yml\n  - openapi/tink-money-manager-api-openapi.yml\n  - openapi/tink-oauth-api-openapi.yml\n  - openapi/tink-payments-api-openapi.yml\n  - openapi/tink-risk-reports-api-openapi.yml\n  - openapi/tink-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/authentication/tink-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Banking
- PSD2
- Payment Initiation
- Account Aggregation
- Risk Decisioning
- Pay by Bank
- Finance
- Banking
- Europe
- Visa
---
