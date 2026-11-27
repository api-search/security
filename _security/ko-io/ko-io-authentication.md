---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ko-io-account-api-openapi.yml
  format: yaml
  label: ko.io Account API
  slug: ko-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-account-api-openapi.yml
- filename: ko-io-bulk-api-openapi.yml
  format: yaml
  label: ko.io Bulk API
  slug: ko-io-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-bulk-api-openapi.yml
- filename: ko-io-congress-api-openapi.yml
  format: yaml
  label: ko.io Congress API
  slug: ko-io-congress-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-congress-api-openapi.yml
- filename: ko-io-crypto-api-openapi.yml
  format: yaml
  label: ko.io Crypto API
  slug: ko-io-crypto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-crypto-api-openapi.yml
- filename: ko-io-dashboards-api-openapi.yml
  format: yaml
  label: ko.io Dashboards API
  slug: ko-io-dashboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-dashboards-api-openapi.yml
- filename: ko-io-europe-api-openapi.yml
  format: yaml
  label: ko.io Europe API
  slug: ko-io-europe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-europe-api-openapi.yml
- filename: ko-io-filings-api-openapi.yml
  format: yaml
  label: ko.io Filings API
  slug: ko-io-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-filings-api-openapi.yml
- filename: ko-io-funds-api-openapi.yml
  format: yaml
  label: ko.io Funds API
  slug: ko-io-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-funds-api-openapi.yml
- filename: ko-io-government-contracts-api-openapi.yml
  format: yaml
  label: ko.io Government contracts API
  slug: ko-io-government-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-government-contracts-api-openapi.yml
- filename: ko-io-insiders-api-openapi.yml
  format: yaml
  label: ko.io Insiders API
  slug: ko-io-insiders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-insiders-api-openapi.yml
- filename: ko-io-institutions-api-openapi.yml
  format: yaml
  label: ko.io Institutions API
  slug: ko-io-institutions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-institutions-api-openapi.yml
- filename: ko-io-macro-api-openapi.yml
  format: yaml
  label: ko.io Macro API
  slug: ko-io-macro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-macro-api-openapi.yml
- filename: ko-io-meta-api-openapi.yml
  format: yaml
  label: ko.io Meta API
  slug: ko-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-meta-api-openapi.yml
- filename: ko-io-research-api-openapi.yml
  format: yaml
  label: ko.io Research API
  slug: ko-io-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-research-api-openapi.yml
- filename: ko-io-search-api-openapi.yml
  format: yaml
  label: ko.io Search API
  slug: ko-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-search-api-openapi.yml
- filename: ko-io-sec-filings-api-openapi.yml
  format: yaml
  label: ko.io SEC Filings API
  slug: ko-io-sec-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-sec-filings-api-openapi.yml
- filename: ko-io-short-data-api-openapi.yml
  format: yaml
  label: ko.io Short Data API
  slug: ko-io-short-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-short-data-api-openapi.yml
- filename: ko-io-stocks-api-openapi.yml
  format: yaml
  label: ko.io Stocks API
  slug: ko-io-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ko-io/openapi/ko-io-stocks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ko.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: ko.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ko.io
provider_slug: ko-io
scheme_count: 1
schemes:
- description: ko.io API key (ko_live_...). Create one at https://ko.io/console/keys/
  name: apiKey
  scheme: bearer
  sources:
  - openapi/ko-io-openapi.yaml
  type: http
slug: ko-io-authentication
source_filename: ko-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/ko-io-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: ko.io API key (ko_live_...). Create one at https://ko.io/console/keys/\n  sources:\n  - openapi/ko-io-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/ko-io/authentication/ko-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Finance
- SEC
- Analytics
- Company
---
