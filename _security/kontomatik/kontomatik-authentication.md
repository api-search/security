---
api_key_in:
- header
api_specs:
- filename: kontomatik-ais-api-openapi.yml
  format: yaml
  label: Kontomatik Account Information Service API
  slug: kontomatik-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-ais-api-openapi.yml
- filename: kontomatik-pdf-parsing-api-openapi.yml
  format: yaml
  label: Kontomatik PDF Parsing API
  slug: kontomatik-pdf-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-pdf-parsing-api-openapi.yml
- filename: kontomatik-data-analysis-api-openapi.yml
  format: yaml
  label: Kontomatik Data Analysis API
  slug: kontomatik-data-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-data-analysis-api-openapi.yml
- filename: kontomatik-report-api-openapi.yml
  format: yaml
  label: Kontomatik Report API
  slug: kontomatik-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-report-api-openapi.yml
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
