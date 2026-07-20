---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Keynua Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keynua secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Keynua
provider_slug: keynua
scheme_count: 2
schemes:
- description: API Key secret value (not the ID). Required on all requests.
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - https://keynua.github.io/slate
  type: apiKey
- description: API Token secret value (not the ID). Required on all requests.
  in: header
  name: authorization
  parameter: authorization
  sources:
  - https://keynua.github.io/slate
  type: apiKey
slug: keynua-authentication
source_filename: keynua-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://keynua.github.io/slate\ndocs: https://keynua.github.io/slate/#authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Every request must carry two header credentials together: x-api-key (the API\n    Key) and authorization (the API Token). Credentials are issued as ID/Secret\n    pairs in the developer settings; the Secret value (not the ID) is sent in each\n    header. Credentials are environment-scoped (separate keys for staging vs\n    production).\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API Key secret value (not the ID). Required on all requests.\n  sources: [https://keynua.github.io/slate]\n- name: authorization\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: API Token secret value (not the ID). Required on all requests.\n  sources: [https://keynua.github.io/slate]\nenvironments:\n\
  - name: production\n  base_url: https://api.keynua.com\n- name: staging\n  base_url: https://api.stg.keynua.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keynua/refs/heads/main/authentication/keynua-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Electronic Signature
- Digital Signature
- Identity Verification
- Biometrics
- KYC
- Onboarding
- OTP
- Webhooks
- Latin America
---
