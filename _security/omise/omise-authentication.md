---
api_key_in: []
api_specs:
- filename: omise-openapi.yml
  format: yaml
  label: Omise Charges API
  slug: omise-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Tokens API
  slug: omise-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Sources API
  slug: omise-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Customers API
  slug: omise-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Refunds API
  slug: omise-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Disputes API
  slug: omise-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Transfers API
  slug: omise-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Recipients API
  slug: omise-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Schedules API
  slug: omise-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Links API
  slug: omise-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Events API
  slug: omise-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
- filename: omise-openapi.yml
  format: yaml
  label: Omise Account and Balance API
  slug: omise-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/openapi/omise-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Omise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Omise secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Omise
provider_slug: omise
scheme_count: 2
schemes:
- description: HTTP Basic authentication against the core API host https://api.omise.co. The account secret key (skey_test_... in test mode, skey_... in live mode) is supplied as the Basic-auth username with an empty password. Used for all server-side operations - charges, customers, refunds, transfers, recipients, schedules, disputes, links, events, account, and balance.
  name: secretKeyAuth
  scheme: basic
  sources:
  - openapi/omise-openapi.yml
  type: http
- description: HTTP Basic authentication against the PCI-scoped vault host https://vault.omise.co (and permitted for creating Sources). The account public key (pkey_test_... / pkey_...) is supplied as the Basic-auth username with an empty password. Used client-side (typically via Omise.js) to tokenize card data so raw PAN never touches your server.
  name: publicKeyAuth
  scheme: basic
  sources:
  - openapi/omise-openapi.yml
  type: http
slug: omise-authentication
source_filename: omise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/omise-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: secretKeyAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication against the core API host https://api.omise.co.\n    The account secret key (skey_test_... in test mode, skey_... in live mode)\n    is supplied as the Basic-auth username with an empty password. Used for all\n    server-side operations - charges, customers, refunds, transfers, recipients,\n    schedules, disputes, links, events, account, and balance.\n  sources:\n  - openapi/omise-openapi.yml\n- name: publicKeyAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication against the PCI-scoped vault host\n    https://vault.omise.co (and permitted for creating Sources). The account\n    public key (pkey_test_... / pkey_...) is supplied as the Basic-auth username\n    with an empty password. Used client-side (typically via Omise.js) to\n\
  \    tokenize card data so raw PAN never touches your server.\n  sources:\n  - openapi/omise-openapi.yml\nnotes: >-\n  Both keys are found on the Opn Payments / Omise dashboard. API behavior can be\n  pinned per-request with the optional Omise-Version header (for example\n  2019-05-29); otherwise the account default API version applies. Keep the\n  secret key server-side only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omise/refs/heads/main/authentication/omise-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Payment Gateway
- Thailand
- Southeast Asia
- Charges
- Tokens
- Sources
- PromptPay
- Cards
- Fintech
---
