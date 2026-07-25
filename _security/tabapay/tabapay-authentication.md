---
api_key_in:
- header
api_specs:
- filename: tabapay-3d-secure-api-openapi.yml
  format: yaml
  label: TabaPay 3D Secure API
  slug: tabapay-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-3d-secure-api-openapi.yml
- filename: tabapay-account-api-openapi.yml
  format: yaml
  label: TabaPay Account API
  slug: tabapay-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-account-api-openapi.yml
- filename: tabapay-bank-api-openapi.yml
  format: yaml
  label: TabaPay Bank API
  slug: tabapay-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-bank-api-openapi.yml
- filename: tabapay-card-api-openapi.yml
  format: yaml
  label: TabaPay Card API
  slug: tabapay-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-card-api-openapi.yml
- filename: tabapay-client-api-openapi.yml
  format: yaml
  label: TabaPay Client API
  slug: tabapay-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-client-api-openapi.yml
- filename: tabapay-fxrate-api-openapi.yml
  format: yaml
  label: TabaPay FXRate API
  slug: tabapay-fxrate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-fxrate-api-openapi.yml
- filename: tabapay-health-api-openapi.yml
  format: yaml
  label: TabaPay Health API
  slug: tabapay-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-health-api-openapi.yml
- filename: tabapay-key-api-openapi.yml
  format: yaml
  label: TabaPay Key API
  slug: tabapay-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-key-api-openapi.yml
- filename: tabapay-ledger-api-openapi.yml
  format: yaml
  label: TabaPay Ledger API
  slug: tabapay-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-ledger-api-openapi.yml
- filename: tabapay-ofac-api-openapi.yml
  format: yaml
  label: TabaPay OFAC API
  slug: tabapay-ofac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-ofac-api-openapi.yml
- filename: tabapay-subclient-api-openapi.yml
  format: yaml
  label: TabaPay SubClient API
  slug: tabapay-subclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-subclient-api-openapi.yml
- filename: tabapay-tag-api-openapi.yml
  format: yaml
  label: TabaPay Tag API
  slug: tabapay-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-tag-api-openapi.yml
- filename: tabapay-transaction-api-openapi.yml
  format: yaml
  label: TabaPay Transaction API
  slug: tabapay-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-transaction-api-openapi.yml
- filename: tabapay-transactionrequest-api-openapi.yml
  format: yaml
  label: TabaPay TransactionRequest API
  slug: tabapay-transactionrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-transactionrequest-api-openapi.yml
- filename: tabapay-user-api-openapi.yml
  format: yaml
  label: TabaPay User API
  slug: tabapay-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-user-api-openapi.yml
- filename: tabapay-verification-api-openapi.yml
  format: yaml
  label: TabaPay Verification API
  slug: tabapay-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-verification-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tabapay Authentication
name_suffix: Authentication
oauth_flows: []
overview: TabaPay secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TabaPay
provider_slug: tabapay
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tabapay-openapi.yml
  type: http
- in: header
  name: custom-header
  parameter: Authorization
  sources:
  - openapi/tabapay-openapi.yml
  type: apiKey
slug: tabapay-authentication
source_filename: tabapay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tabapay-openapi.yml + https://developers.tabapay.com/reference/getting-started\ndocs: https://developers.tabapay.com/reference/getting-started\nnotes: TabaPay APIs are not publicly self-serve — a static bearer access token (API key) is\n  issued at boarding along with a client-specific FQDN, and requests must come from allowlisted\n  IPs (sandbox and production IPs must differ). Expired sandbox credentials are renewed via\n  help@tabapay.com. Card data may additionally be RSA-encrypted client-side using keys managed\n  through the Key API (keyCreate/keyRetrieve/keyDelete).\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/tabapay-openapi.yml\n- name: custom-header\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/tabapay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/authentication/tabapay-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Fintech
- Payments
- Instant Payments
- Money Movement
- Payouts
- Cards
- Real-Time Payments
- ACH
---
