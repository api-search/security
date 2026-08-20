---
api_key_in:
- header
- query
api_specs:
- filename: 73-strings-asset-info-api-openapi.yml
  format: yaml
  label: 73 Strings Asset Info API
  slug: 73-strings-asset-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-asset-info-api-openapi.yml
- filename: 73-strings-captable-api-openapi.yml
  format: yaml
  label: 73 Strings Captable API
  slug: 73-strings-captable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-captable-api-openapi.yml
- filename: 73-strings-documents-api-openapi.yml
  format: yaml
  label: 73 Strings Documents API
  slug: 73-strings-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-documents-api-openapi.yml
- filename: 73-strings-financial-data-api-openapi.yml
  format: yaml
  label: 73 Strings Financial Data API
  slug: 73-strings-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-financial-data-api-openapi.yml
- filename: 73-strings-qualitative-data-api-openapi.yml
  format: yaml
  label: 73 Strings Qualitative Data API
  slug: 73-strings-qualitative-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-qualitative-data-api-openapi.yml
- filename: 73-strings-transaction-api-api-openapi.yml
  format: yaml
  label: 73 Strings Transaction API API
  slug: 73-strings-transaction-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-transaction-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: 73 Strings Authentication
name_suffix: Authentication
oauth_flows: []
overview: 73 Strings secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 73 Strings
provider_slug: 73-strings
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: subscription-key
  sources:
  - openapi/73-strings-asset-info-openapi.yml
  - openapi/73-strings-captable-openapi.yml
  - openapi/73-strings-documents-openapi.yml
  - openapi/73-strings-financial-data-openapi.yml
  - openapi/73-strings-qualitative-data-openapi.yml
  - openapi/73-strings-transaction-api-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/73-strings-asset-info-openapi.yml
  - openapi/73-strings-captable-openapi.yml
  - openapi/73-strings-documents-openapi.yml
  - openapi/73-strings-financial-data-openapi.yml
  - openapi/73-strings-qualitative-data-openapi.yml
  - openapi/73-strings-transaction-api-openapi.yml
  type: apiKey
slug: 73-strings-authentication
source_filename: 73-strings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/73-strings-asset-info-openapi.yml, openapi/73-strings-captable-openapi.yml,\n  openapi/73-strings-documents-openapi.yml, openapi/73-strings-financial-data-openapi.yml, openapi/73-strings-qualitative-data-openapi.yml,\n  openapi/73-strings-transaction-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: subscription-key\n  sources:\n  - openapi/73-strings-asset-info-openapi.yml\n  - openapi/73-strings-captable-openapi.yml\n  - openapi/73-strings-documents-openapi.yml\n  - openapi/73-strings-financial-data-openapi.yml\n  - openapi/73-strings-qualitative-data-openapi.yml\n  - openapi/73-strings-transaction-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/73-strings-asset-info-openapi.yml\n  - openapi/73-strings-captable-openapi.yml\n  - openapi/73-strings-documents-openapi.yml\n\
  \  - openapi/73-strings-financial-data-openapi.yml\n  - openapi/73-strings-qualitative-data-openapi.yml\n  - openapi/73-strings-transaction-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/authentication/73-strings-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Private Markets
- Valuation
- Portfolio Monitoring
- Private Equity
- Private Credit
- Venture Capital
- Alternative Assets
- Financial Data
- Data Extraction
- Fintech
- Asset Management
- Azure API Management
---
