---
api_key_in:
- header
api_specs:
- filename: international-trade-administration-consolidated-screening-list-api-openapi.yml
  format: yaml
  label: International Trade Administration Consolidated Screening List API
  slug: international-trade-administration-consolidated-screening-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-consolidated-screening-list-api-openapi.yml
- filename: international-trade-administration-country-commercial-guides-api-openapi.yml
  format: yaml
  label: International Trade Administration Country Commercial Guides API
  slug: international-trade-administration-country-commercial-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-country-commercial-guides-api-openapi.yml
- filename: international-trade-administration-customs-tariff-api-openapi.yml
  format: yaml
  label: International Trade Administration Customs Tariff API
  slug: international-trade-administration-customs-tariff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-customs-tariff-api-openapi.yml
- filename: international-trade-administration-de-minimis-api-openapi.yml
  format: yaml
  label: International Trade Administration De Minimis API
  slug: international-trade-administration-de-minimis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-de-minimis-api-openapi.yml
- filename: international-trade-administration-market-intelligence-api-openapi.yml
  format: yaml
  label: International Trade Administration Market Intelligence API
  slug: international-trade-administration-market-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-market-intelligence-api-openapi.yml
- filename: international-trade-administration-trade-events-api-openapi.yml
  format: yaml
  label: International Trade Administration Trade Events API
  slug: international-trade-administration-trade-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-trade-events-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: International Trade Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: International Trade Administration secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: International Trade Administration
provider_slug: international-trade-administration
scheme_count: 1
schemes:
- description: ITA APIs require an Ocp-Apim Subscription Key obtained from the developer.trade.gov portal.
  in: header
  name: subscriptionKey
  parameter: subscription-key
  sources:
  - openapi/international-trade-administration-openapi.yml
  type: apiKey
slug: international-trade-administration-authentication
source_filename: international-trade-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/international-trade-administration-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter: subscription-key\n  description: ITA APIs require an Ocp-Apim Subscription Key obtained from the developer.trade.gov\n    portal.\n  sources:\n  - openapi/international-trade-administration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/authentication/international-trade-administration-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Customs
- Export
- Federal Government
- International Business
- Screening List
- Tariffs
- Trade
- Trade Data
- Trade Events
---
