---
api_key_in:
- header
api_specs:
- filename: hibp-openapi.yml
  format: yaml
  label: HIBP API v3
  slug: hibp-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/hibp-openapi.yml
- filename: pwned-passwords-openapi.yml
  format: yaml
  label: Pwned Passwords
  slug: pwned-passwords
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/pwned-passwords-openapi.yml
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
