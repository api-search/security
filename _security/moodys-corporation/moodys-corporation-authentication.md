---
api_key_in:
- header
api_specs:
- filename: moodys-analytics-developer-openapi.yml
  format: yaml
  label: Moody's Analytics Developer Platform
  slug: developer-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-corporation/refs/heads/main/openapi/moodys-analytics-developer-openapi.yml
- filename: moodys-data-buffet-api-openapi.yml
  format: yaml
  label: Moody's Analytics Data Buffet API
  slug: data-buffet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-corporation/refs/heads/main/openapi/moodys-data-buffet-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Moodys Corporation Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Moody's Corporation secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Moody's Corporation
provider_slug: moodys-corporation
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.economy.com/oauth2/token
  name: oauth2
  sources:
  - openapi/moodys-analytics-developer-openapi.yml
  - openapi/moodys-data-buffet-api-openapi.yml
  type: oauth2
- description: HMAC-SHA256 request signing scheme used as an alternative to OAuth2 on legacy Moody's Analytics product APIs (Data Buffet, Scenario Studio).
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/moodys-analytics-developer-openapi.yml
  type: apiKey
slug: moodys-corporation-authentication
source_filename: moodys-corporation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moodys-analytics-developer-openapi.yml, openapi/moodys-data-buffet-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/moodys-analytics-developer-openapi.yml\n  - openapi/moodys-data-buffet-api-openapi.yml\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC-SHA256 request signing scheme used as an alternative to OAuth2 on legacy\n    Moody's Analytics product APIs (Data Buffet, Scenario Studio).\n  sources:\n  - openapi/moodys-analytics-developer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys-corporation/refs/heads/main/authentication/moodys-corporation-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Analytics
- Catastrophe Risk
- Climate Risk
- Compliance
- Credit Ratings
- Economic Data
- ESG
- Financial Data
- KYC
- Risk
- Fortune 1000
---
