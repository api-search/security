---
api_key_in:
- header
api_specs:
- filename: ledger-investing-analytics-openapi.yml
  format: yaml
  label: Ledger Analytics API
  slug: analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledger-investing/refs/heads/main/openapi/ledger-investing-analytics-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ledger Investing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ledger Investing secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ledger Investing
provider_slug: ledger-investing
scheme_count: 1
schemes:
- description: The Ledger Analytics API authenticates with a single opaque API key sent in the Authorization header using the custom `Api-Key` scheme (not Bearer). There is no OAuth, OIDC or mTLS surface. The first-party Python client reads the key from the LEDGER_ANALYTICS_API_KEY environment variable and sets the header for every request.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/ledger-investing-analytics-openapi.yml
  type: apiKey
  value_format: Api-Key <API_KEY>
slug: ledger-investing-authentication
source_filename: ledger-investing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/ledger-investing-analytics-openapi.yml\ndocs: https://ledger-investing-ledger-analytics.readthedocs-hosted.com/en/stable/apikeys.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  scopes: none\n  mtls: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: 'Api-Key <API_KEY>'\n  description: >-\n    The Ledger Analytics API authenticates with a single opaque API key sent in the\n    Authorization header using the custom `Api-Key` scheme (not Bearer). There is no OAuth,\n    OIDC or mTLS surface. The first-party Python client reads the key from the\n    LEDGER_ANALYTICS_API_KEY environment variable and sets the header for every request.\n  sources: [openapi/ledger-investing-analytics-openapi.yml]\naccess:\n  status: beta\n  request_process: Email analytics@ledgerinvesting.com to sign up for an account and request a key.\n  key_management:\
  \ https://ldgr.app/api-keys\n  environment_variables:\n  - {name: LEDGER_ANALYTICS_API_KEY, environment: production, host: 'https://api.korra.com/analytics/'}\n  - {name: LEDGER_ANALYTICS_DEV_API_KEY, environment: development, note: internal Ledger/Korra development host}\n  - {name: LEDGER_ANALYTICS_LOCAL_API_KEY, environment: local, note: localhost development only}\n  environment_selector: LEDGER_ANALYTICS_ENV (PROD | DEV | LOCAL, default PROD)\nfailure_modes:\n- {status: 403, meaning: The API key does not have permission to perform this action.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledger-investing/refs/heads/main/authentication/ledger-investing-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Insurance Tech
- Insurance
- Reinsurance
- Insurance-Linked Securities
- Actuarial
- Analytics
- Capital Markets
- Data Science
- Financial Services
---
