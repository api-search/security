---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: opencapital-sh-business-profiles-api-openapi.yml
  format: yaml
  label: OpenCapital Business profiles API
  slug: opencapital-sh-business-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-business-profiles-api-openapi.yml
- filename: opencapital-sh-companies-api-openapi.yml
  format: yaml
  label: OpenCapital Companies API
  slug: opencapital-sh-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-companies-api-openapi.yml
- filename: opencapital-sh-filings-api-openapi.yml
  format: yaml
  label: OpenCapital Filings API
  slug: opencapital-sh-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-filings-api-openapi.yml
- filename: opencapital-sh-metrics-and-segments-api-openapi.yml
  format: yaml
  label: OpenCapital Metrics and segments API
  slug: opencapital-sh-metrics-and-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-metrics-and-segments-api-openapi.yml
- filename: opencapital-sh-reported-earnings-api-openapi.yml
  format: yaml
  label: OpenCapital Reported earnings API
  slug: opencapital-sh-reported-earnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-reported-earnings-api-openapi.yml
- filename: opencapital-sh-screening-api-openapi.yml
  format: yaml
  label: OpenCapital Screening API
  slug: opencapital-sh-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-screening-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: OpenCapital Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenCapital secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenCapital
provider_slug: opencapital-sh
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/opencapital-sh-openapi.json
  type: http
- in: header
  name: applicationKey
  parameter: x-api-key
  sources:
  - openapi/opencapital-sh-openapi.json
  type: apiKey
slug: opencapital-sh-authentication
source_filename: opencapital-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/opencapital-sh-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/opencapital-sh-openapi.json\n- name: applicationKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/opencapital-sh-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/opencapital-sh/authentication/opencapital-sh-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- SEC Filings
- Financial Data
- Earnings
- Company screener
---
