---
api_key_in: []
api_specs:
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Hosted Payment Page API
  slug: paytabs-hosted-payment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Managed Form API
  slug: paytabs-managed-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Own Form API
  slug: paytabs-own-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Transaction Management API
  slug: paytabs-transaction-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Token & Recurring Billing API
  slug: paytabs-token-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Invoices API
  slug: paytabs-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Paytabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayTabs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PayTabs
provider_slug: paytabs
scheme_count: 2
schemes:
- format: server key (e.g. SXXXXXXXXX-XXXXXXXXXX-XXXXXXXXXX)
  header: authorization
  in: header
  name: server_key
  sources:
  - openapi/paytabs-openapi.yml
  - https://support.paytabs.com/en/support/solutions/articles/60000709801-how-to-get-my-authentication-integration-api-keys-
  type: apiKey
- format: CXXXXXXXXX-XXXXXXXXXX-XXXXXXXXXX
  header: client key
  in: header
  name: client_key
  sources:
  - https://support.paytabs.com/en/support/solutions/articles/60000709773-authentication-integration-api-keys
  type: apiKey
  usage: Browser-side own-form and card tokenization; paired with profile_id.
slug: paytabs-authentication
source_filename: paytabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/paytabs-openapi.yml\nsummary:\n  types:\n  - apiKey\nnotes: >-\n  PayTabs PT2 authenticates server-to-server calls with a merchant server key\n  sent as the raw value of the `authorization` HTTP header (NOT an OAuth/Bearer\n  token). The `profile_id` in the request body identifies which profile the\n  server key acts on. A separate client key is used for browser-side own-form /\n  tokenization. Keys are region-scoped: a key must be used against the host that\n  matches its region (e.g. secure.paytabs.sa for KSA) or authentication fails.\nschemes:\n- name: server_key\n  type: apiKey\n  in: header\n  header: authorization\n  format: server key (e.g. SXXXXXXXXX-XXXXXXXXXX-XXXXXXXXXX)\n  sources:\n  - openapi/paytabs-openapi.yml\n  - https://support.paytabs.com/en/support/solutions/articles/60000709801-how-to-get-my-authentication-integration-api-keys-\n- name: client_key\n  type: apiKey\n  in: header\n  header: client key\n\
  \  format: CXXXXXXXXX-XXXXXXXXXX-XXXXXXXXXX\n  usage: Browser-side own-form and card tokenization; paired with profile_id.\n  sources:\n  - https://support.paytabs.com/en/support/solutions/articles/60000709773-authentication-integration-api-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/authentication/paytabs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- Saudi Arabia
- Cards
- mada
---
