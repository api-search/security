---
api_key_in:
- header
api_specs:
- filename: kontomatik-aggregation-api-openapi.yml
  format: yaml
  label: Kontomatik Aggregation API
  slug: kontomatik-aggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-aggregation-api-openapi.yml
- filename: kontomatik-catalog-api-openapi.yml
  format: yaml
  label: Kontomatik Catalog API
  slug: kontomatik-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-catalog-api-openapi.yml
- filename: kontomatik-command-api-openapi.yml
  format: yaml
  label: Kontomatik Command API
  slug: kontomatik-command-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-command-api-openapi.yml
- filename: kontomatik-confirmations-api-openapi.yml
  format: yaml
  label: Kontomatik Confirmations API
  slug: kontomatik-confirmations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-confirmations-api-openapi.yml
- filename: kontomatik-features-api-openapi.yml
  format: yaml
  label: Kontomatik Features API
  slug: kontomatik-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-features-api-openapi.yml
- filename: kontomatik-income-api-openapi.yml
  format: yaml
  label: Kontomatik Income API
  slug: kontomatik-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-income-api-openapi.yml
- filename: kontomatik-labeling-api-openapi.yml
  format: yaml
  label: Kontomatik Labeling API
  slug: kontomatik-labeling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-labeling-api-openapi.yml
- filename: kontomatik-mock-api-openapi.yml
  format: yaml
  label: Kontomatik Mock API
  slug: kontomatik-mock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-mock-api-openapi.yml
- filename: kontomatik-owner-api-openapi.yml
  format: yaml
  label: Kontomatik Owner API
  slug: kontomatik-owner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-owner-api-openapi.yml
- filename: kontomatik-profile-api-openapi.yml
  format: yaml
  label: Kontomatik Profile API
  slug: kontomatik-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-profile-api-openapi.yml
- filename: kontomatik-reports-api-openapi.yml
  format: yaml
  label: Kontomatik Reports API
  slug: kontomatik-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-reports-api-openapi.yml
- filename: kontomatik-score-api-openapi.yml
  format: yaml
  label: Kontomatik Score API
  slug: kontomatik-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-score-api-openapi.yml
- filename: kontomatik-signin-api-openapi.yml
  format: yaml
  label: Kontomatik SignIn API
  slug: kontomatik-signin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-signin-api-openapi.yml
- filename: kontomatik-statements-api-openapi.yml
  format: yaml
  label: Kontomatik Statements API
  slug: kontomatik-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-statements-api-openapi.yml
- filename: kontomatik-summary-api-openapi.yml
  format: yaml
  label: Kontomatik Summary API
  slug: kontomatik-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-summary-api-openapi.yml
- filename: kontomatik-vendors-api-openapi.yml
  format: yaml
  label: Kontomatik Vendors API
  slug: kontomatik-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-vendors-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kontomatik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kontomatik secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kontomatik
provider_slug: kontomatik
scheme_count: 1
schemes:
- description: API key issued by Kontomatik; requests must originate from a whitelisted server.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/kontomatik-ais-api-openapi.yml
  - openapi/kontomatik-data-analysis-api-openapi.yml
  - openapi/kontomatik-pdf-parsing-api-openapi.yml
  - openapi/kontomatik-report-api-openapi.yml
  type: apiKey
slug: kontomatik-authentication
source_filename: kontomatik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kontomatik-ais-api-openapi.yml, openapi/kontomatik-data-analysis-api-openapi.yml,\n  openapi/kontomatik-pdf-parsing-api-openapi.yml, openapi/kontomatik-report-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key issued by Kontomatik; requests must originate from a whitelisted server.\n  sources:\n  - openapi/kontomatik-ais-api-openapi.yml\n  - openapi/kontomatik-data-analysis-api-openapi.yml\n  - openapi/kontomatik-pdf-parsing-api-openapi.yml\n  - openapi/kontomatik-report-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/authentication/kontomatik-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Open Banking
- PSD2
- AIS
- Bank Data Aggregation
- CEE
- KYC
- Credit Scoring
- Transaction Labeling
- PDF Parsing
---
