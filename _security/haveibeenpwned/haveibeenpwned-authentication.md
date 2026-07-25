---
api_key_in:
- header
api_specs:
- filename: haveibeenpwned-breached-accounts-api-openapi.yml
  format: yaml
  label: HaveIBeenPwned Breached Accounts API
  slug: haveibeenpwned-breached-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/haveibeenpwned-breached-accounts-api-openapi.yml
- filename: haveibeenpwned-breaches-api-openapi.yml
  format: yaml
  label: HaveIBeenPwned Breaches API
  slug: haveibeenpwned-breaches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/haveibeenpwned-breaches-api-openapi.yml
- filename: haveibeenpwned-data-classes-api-openapi.yml
  format: yaml
  label: HaveIBeenPwned Data Classes API
  slug: haveibeenpwned-data-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/haveibeenpwned-data-classes-api-openapi.yml
- filename: haveibeenpwned-domain-search-api-openapi.yml
  format: yaml
  label: HaveIBeenPwned Domain Search API
  slug: haveibeenpwned-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/haveibeenpwned-domain-search-api-openapi.yml
- filename: haveibeenpwned-pastes-api-openapi.yml
  format: yaml
  label: HaveIBeenPwned Pastes API
  slug: haveibeenpwned-pastes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/haveibeenpwned-pastes-api-openapi.yml
- filename: haveibeenpwned-range-search-api-openapi.yml
  format: yaml
  label: HaveIBeenPwned Range Search API
  slug: haveibeenpwned-range-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/haveibeenpwned-range-search-api-openapi.yml
- filename: haveibeenpwned-stealer-logs-api-openapi.yml
  format: yaml
  label: HaveIBeenPwned Stealer Logs API
  slug: haveibeenpwned-stealer-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/haveibeenpwned-stealer-logs-api-openapi.yml
- filename: haveibeenpwned-subscription-api-openapi.yml
  format: yaml
  label: HaveIBeenPwned Subscription API
  slug: haveibeenpwned-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/haveibeenpwned-subscription-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Haveibeenpwned Authentication
name_suffix: Authentication
oauth_flows: []
overview: HaveIBeenPwned secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HaveIBeenPwned
provider_slug: haveibeenpwned
scheme_count: 1
schemes:
- description: '32-character hexadecimal API key issued at https://haveibeenpwned.com/API/Key.

    Required for all account, paste, stealer log, domain search, and subscription endpoints.'
  in: header
  name: ApiKeyAuth
  parameter: hibp-api-key
  sources:
  - openapi/hibp-openapi.yml
  type: apiKey
slug: haveibeenpwned-authentication
source_filename: haveibeenpwned-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hibp-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: hibp-api-key\n  description: |-\n    32-character hexadecimal API key issued at https://haveibeenpwned.com/API/Key.\n    Required for all account, paste, stealer log, domain search, and subscription endpoints.\n  sources:\n  - openapi/hibp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/authentication/haveibeenpwned-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Breach Notification
- Credential Stuffing
- Stealer Logs
- K-Anonymity
- Privacy
- Identity
---
