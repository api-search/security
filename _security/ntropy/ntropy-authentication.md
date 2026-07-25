---
api_key_in:
- header
api_specs:
- filename: ntropy-account-holder-api-openapi.yml
  format: yaml
  label: Ntropy Account Holder API
  slug: ntropy-account-holder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-account-holder-api-openapi.yml
- filename: ntropy-accountholders-api-openapi.yml
  format: yaml
  label: Ntropy accountHolders API
  slug: ntropy-accountholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-accountholders-api-openapi.yml
- filename: ntropy-bank-statements-api-openapi.yml
  format: yaml
  label: Ntropy Bank statements API
  slug: ntropy-bank-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-bank-statements-api-openapi.yml
- filename: ntropy-bankstatements-api-openapi.yml
  format: yaml
  label: Ntropy bankStatements API
  slug: ntropy-bankstatements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-bankstatements-api-openapi.yml
- filename: ntropy-batches-api-openapi.yml
  format: yaml
  label: Ntropy batches API
  slug: ntropy-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-batches-api-openapi.yml
- filename: ntropy-categories-api-openapi.yml
  format: yaml
  label: Ntropy categories API
  slug: ntropy-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-categories-api-openapi.yml
- filename: ntropy-enrichment-api-openapi.yml
  format: yaml
  label: Ntropy Enrichment API
  slug: ntropy-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-enrichment-api-openapi.yml
- filename: ntropy-entities-api-openapi.yml
  format: yaml
  label: Ntropy entities API
  slug: ntropy-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-entities-api-openapi.yml
- filename: ntropy-labels-api-openapi.yml
  format: yaml
  label: Ntropy Labels API
  slug: ntropy-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-labels-api-openapi.yml
- filename: ntropy-misc-api-openapi.yml
  format: yaml
  label: Ntropy Misc API
  slug: ntropy-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-misc-api-openapi.yml
- filename: ntropy-personalization-api-openapi.yml
  format: yaml
  label: Ntropy personalization API
  slug: ntropy-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-personalization-api-openapi.yml
- filename: ntropy-recurrence-api-openapi.yml
  format: yaml
  label: Ntropy recurrence API
  slug: ntropy-recurrence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-recurrence-api-openapi.yml
- filename: ntropy-reporting-api-openapi.yml
  format: yaml
  label: Ntropy Reporting API
  slug: ntropy-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-reporting-api-openapi.yml
- filename: ntropy-reports-api-openapi.yml
  format: yaml
  label: Ntropy reports API
  slug: ntropy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-reports-api-openapi.yml
- filename: ntropy-transactions-api-openapi.yml
  format: yaml
  label: Ntropy transactions API
  slug: ntropy-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-transactions-api-openapi.yml
- filename: ntropy-webhooks-api-openapi.yml
  format: yaml
  label: Ntropy webhooks API
  slug: ntropy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/openapi/ntropy-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ntropy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ntropy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ntropy
provider_slug: ntropy
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/ntropy-api-v3-openapi-original.json
  - openapi/ntropy-transaction-api-openapi-original.json
  type: apiKey
slug: ntropy-authentication
source_filename: ntropy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/ntropy-api-v3-openapi-original.json, openapi/ntropy-transaction-api-openapi-original.json\ndocs: https://docs.ntropy.com/api/auth\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Single auth mechanism: an API key sent in the X-API-KEY request header. Keys are\n    created, disabled and rotated in the dashboard (https://dashboard.ntropy.com/keys).\n    Rotating a key changes only its authorization; previously submitted data stays\n    accessible. No OAuth/OIDC.\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/ntropy-api-v3-openapi-original.json\n  - openapi/ntropy-transaction-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntropy/refs/heads/main/authentication/ntropy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Transaction Enrichment
- Financial Data
- Data Enrichment
- Bank Statements
- Categorization
- Underwriting
---
