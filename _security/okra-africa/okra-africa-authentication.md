---
api_key_in: []
api_specs:
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Auth API
  slug: okra-africa-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Accounts API
  slug: okra-africa-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Balance API
  slug: okra-africa-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Transactions API
  slug: okra-africa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Identity API
  slug: okra-africa-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Income API
  slug: okra-africa-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Verification (KYC) API
  slug: okra-africa-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Payments API
  slug: okra-africa-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Banks API
  slug: okra-africa-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Customers API
  slug: okra-africa-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Wallet API
  slug: okra-africa-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Reports API
  slug: okra-africa-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Okra Africa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Okra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Okra
provider_slug: okra-africa
scheme_count: 1
schemes:
- description: 'Okra Secret key, sent as `Authorization: Bearer <secret>`. The secret was issued in the Okra dashboard (https://dash.okra.ng/settings/api-keys) and a separate key existed per environment (production vs sandbox). Confirmed from the official okraHQ/okra-node SDK request wrapper (src/utils/req-wrapper.js). RETIRED - the auth host no longer resolves.'
  name: okraSecret
  scheme: bearer
  sources:
  - openapi/okra-africa-openapi.yml
  - https://github.com/okraHQ/okra-node
  type: http
slug: okra-africa-authentication
source_filename: okra-africa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/okra-africa-openapi.yml\nstatus: retired\nsummary:\n  types:\n  - http\nschemes:\n- name: okraSecret\n  type: http\n  scheme: bearer\n  description: >-\n    Okra Secret key, sent as `Authorization: Bearer <secret>`. The secret was\n    issued in the Okra dashboard (https://dash.okra.ng/settings/api-keys) and a\n    separate key existed per environment (production vs sandbox). Confirmed from\n    the official okraHQ/okra-node SDK request wrapper\n    (src/utils/req-wrapper.js). RETIRED - the auth host no longer resolves.\n  sources:\n  - openapi/okra-africa-openapi.yml\n  - https://github.com/okraHQ/okra-node\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/authentication/okra-africa-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Banking
- Open Finance
- Financial Data
- Payments
- Fintech
- Account Linking
- Bank Data
- Africa
- Nigeria
- Financial Infrastructure
- Retired
---
