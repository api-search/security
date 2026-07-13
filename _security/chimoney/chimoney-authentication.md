---
api_key_in: []
api_specs:
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Payouts API
  slug: chimoney-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Wallets API
  slug: chimoney-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Multicurrency Wallets API
  slug: chimoney-multicurrency-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Sub-Accounts API
  slug: chimoney-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Redeem API
  slug: chimoney-redeem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Info API
  slug: chimoney-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Accounts API
  slug: chimoney-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Payments API
  slug: chimoney-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chimoney Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chimoney secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chimoney
provider_slug: chimoney
scheme_count: 1
schemes:
- description: API key issued self-serve from the Chimoney developer dashboard (https://dash.chimoney.io/developers). Passed on every request in the `X-API-KEY` HTTP header. A separate sandbox key and host (https://api-v2-sandbox.chimoney.io) are available for testing; production is https://api.chimoney.io.
  in: header
  name: apiKeyAuth
  parameterName: X-API-KEY
  sources:
  - openapi/chimoney-openapi.yml
  - https://chimoney.readme.io/reference/authentication
  type: apiKey
slug: chimoney-authentication
source_filename: chimoney-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/chimoney-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameterName: X-API-KEY\n  description: 'API key issued self-serve from the Chimoney developer dashboard\n    (https://dash.chimoney.io/developers). Passed on every request in the `X-API-KEY`\n    HTTP header. A separate sandbox key and host (https://api-v2-sandbox.chimoney.io)\n    are available for testing; production is https://api.chimoney.io.'\n  sources:\n  - openapi/chimoney-openapi.yml\n  - https://chimoney.readme.io/reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/authentication/chimoney-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payouts
- Disbursements
- Payments
- Africa
- Global Payouts
- Wallets
- Multicurrency
- Gift Cards
- Mobile Money
- Fintech
---
