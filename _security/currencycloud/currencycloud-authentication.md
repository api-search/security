---
api_key_in:
- header
api_specs:
- filename: currencycloud-openapi-original.yml
  format: yaml
  label: Currencycloud API v2
  slug: currencycloud-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencycloud/refs/heads/main/openapi/currencycloud-openapi-original.yml
- filename: currencycloud-onboarding-openapi-original.yml
  format: yaml
  label: Currencycloud Onboarding API (beta pilot)
  slug: currencycloud-onboarding-api-beta-pilot
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencycloud/refs/heads/main/openapi/currencycloud-onboarding-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Currencycloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Currencycloud secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Currencycloud
provider_slug: currencycloud
scheme_count: 1
schemes:
- in: header
  name: AuthToken
  parameter: X-Auth-Token
  sources:
  - openapi/currencycloud-onboarding-openapi-original.yml
  type: apiKey
slug: currencycloud-authentication
source_filename: currencycloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/currencycloud-onboarding-openapi-original.yml\ndocs: https://developer.currencycloud.com/guides/integration-guides/authentication/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  style: login-token\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/currencycloud-onboarding-openapi-original.yml\nflow:\n  description: >-\n    All endpoints require authentication. Exchange long-lived credentials for a\n    short-lived session token, then pass the token on every request.\n  steps:\n    - Call POST /v2/authenticate/api with form-data login_id (usually your email)\n      and api_key (64-char key from the developer portal).\n    - Extract auth_token from the JSON response.\n    - Send the token as the X-Auth-Token header on all subsequent calls.\n    - Call POST /v2/authenticate/close_session to terminate the session.\n  token_expiry: 30 minutes of inactivity\
  \ (then HTTP 401 auth_failed)\n  api_key_length: 64 characters\n  on_behalf_of: >-\n    House accounts can act for sub-accounts by passing on_behalf_of (a\n    sub-account contact id) on supported operations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencycloud/refs/heads/main/authentication/currencycloud-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Payments
- Foreign Exchange
- Cross-Border Payments
- Money Transfer
- Currency Conversion
- Banking
---
