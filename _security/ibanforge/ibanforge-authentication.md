---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: ibanforge-api-keys-api-openapi.yml
  format: yaml
  label: IBANforge API Keys API
  slug: ibanforge-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-api-keys-api-openapi.yml
- filename: ibanforge-bic-api-openapi.yml
  format: yaml
  label: IBANforge BIC API
  slug: ibanforge-bic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-bic-api-openapi.yml
- filename: ibanforge-compliance-api-openapi.yml
  format: yaml
  label: IBANforge Compliance API
  slug: ibanforge-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-compliance-api-openapi.yml
- filename: ibanforge-credits-api-openapi.yml
  format: yaml
  label: IBANforge Credits API
  slug: ibanforge-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-credits-api-openapi.yml
- filename: ibanforge-free-api-openapi.yml
  format: yaml
  label: IBANforge Free API
  slug: ibanforge-free-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-free-api-openapi.yml
- filename: ibanforge-iban-api-openapi.yml
  format: yaml
  label: IBANforge IBAN API
  slug: ibanforge-iban-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-iban-api-openapi.yml
- filename: ibanforge-mcp-api-openapi.yml
  format: yaml
  label: IBANforge MCP API
  slug: ibanforge-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-mcp-api-openapi.yml
- filename: ibanforge-swiss-clearing-api-openapi.yml
  format: yaml
  label: IBANforge Swiss Clearing API
  slug: ibanforge-swiss-clearing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-swiss-clearing-api-openapi.yml
- filename: ibanforge-account-api-openapi.yml
  format: yaml
  label: IBANforge Account API
  slug: ibanforge-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-account-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Ibanforge Authentication
name_suffix: Authentication
oauth_flows: []
overview: IBANforge secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IBANforge
provider_slug: ibanforge
scheme_count: 3
schemes:
- description: x402 USDC micropayment signature (protocol v2). Clients holding v1 payment requirements may send the same signature as X-Payment; both are accepted.
  in: header
  name: x402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/ibanforge-account-api-openapi.yml
  - openapi/ibanforge-api-keys-api-openapi.yml
  - openapi/ibanforge-bic-api-openapi.yml
  - openapi/ibanforge-compliance-api-openapi.yml
  - openapi/ibanforge-credits-api-openapi.yml
  - openapi/ibanforge-free-api-openapi.yml
  - openapi/ibanforge-iban-api-openapi.yml
  - openapi/ibanforge-mcp-api-openapi.yml
  - openapi/ibanforge-swiss-clearing-api-openapi.yml
  type: apiKey
- description: API key (Bearer ifk_xxx) — 25 free requests/month without an email address, 200 a month once claimed, or a custom quota for paid keys
  name: apiKey
  scheme: bearer
  sources:
  - openapi/ibanforge-account-api-openapi.yml
  - openapi/ibanforge-api-keys-api-openapi.yml
  - openapi/ibanforge-bic-api-openapi.yml
  - openapi/ibanforge-compliance-api-openapi.yml
  - openapi/ibanforge-credits-api-openapi.yml
  - openapi/ibanforge-free-api-openapi.yml
  - openapi/ibanforge-iban-api-openapi.yml
  - openapi/ibanforge-mcp-api-openapi.yml
  - openapi/ibanforge-swiss-clearing-api-openapi.yml
  type: http
- description: 'Session of the account page, set by POST /v1/account/session: HttpOnly, Secure, SameSite=Strict, Path=/v1/account, 7 days from sign-in. Read-only: it opens no paid route and no route that acts on a key.'
  in: cookie
  name: accountSession
  parameter: ibanforge_account
  sources:
  - openapi/ibanforge-account-api-openapi.yml
  - openapi/ibanforge-api-keys-api-openapi.yml
  - openapi/ibanforge-bic-api-openapi.yml
  - openapi/ibanforge-compliance-api-openapi.yml
  - openapi/ibanforge-credits-api-openapi.yml
  - openapi/ibanforge-free-api-openapi.yml
  - openapi/ibanforge-iban-api-openapi.yml
  - openapi/ibanforge-mcp-api-openapi.yml
  - openapi/ibanforge-swiss-clearing-api-openapi.yml
  type: apiKey
slug: ibanforge-authentication
source_filename: ibanforge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: derived\nsource: openapi/ibanforge-account-api-openapi.yml, openapi/ibanforge-api-keys-api-openapi.yml,\n  openapi/ibanforge-bic-api-openapi.yml, openapi/ibanforge-compliance-api-openapi.yml, openapi/ibanforge-credits-api-openapi.yml,\n  openapi/ibanforge-free-api-openapi.yml, openapi/ibanforge-iban-api-openapi.yml, openapi/ibanforge-mcp-api-openapi.yml,\n  openapi/ibanforge-swiss-clearing-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 USDC micropayment signature (protocol v2). Clients holding v1 payment requirements\n    may send the same signature as X-Payment; both are accepted.\n  sources:\n  - openapi/ibanforge-account-api-openapi.yml\n  - openapi/ibanforge-api-keys-api-openapi.yml\n  - openapi/ibanforge-bic-api-openapi.yml\n  - openapi/ibanforge-compliance-api-openapi.yml\n\
  \  - openapi/ibanforge-credits-api-openapi.yml\n  - openapi/ibanforge-free-api-openapi.yml\n  - openapi/ibanforge-iban-api-openapi.yml\n  - openapi/ibanforge-mcp-api-openapi.yml\n  - openapi/ibanforge-swiss-clearing-api-openapi.yml\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key (Bearer ifk_xxx) — 25 free requests/month without an email address, 200\n    a month once claimed, or a custom quota for paid keys\n  sources:\n  - openapi/ibanforge-account-api-openapi.yml\n  - openapi/ibanforge-api-keys-api-openapi.yml\n  - openapi/ibanforge-bic-api-openapi.yml\n  - openapi/ibanforge-compliance-api-openapi.yml\n  - openapi/ibanforge-credits-api-openapi.yml\n  - openapi/ibanforge-free-api-openapi.yml\n  - openapi/ibanforge-iban-api-openapi.yml\n  - openapi/ibanforge-mcp-api-openapi.yml\n  - openapi/ibanforge-swiss-clearing-api-openapi.yml\n- name: accountSession\n  type: apiKey\n  in: cookie\n  parameter: ibanforge_account\n  description: 'Session of the account page, set\
  \ by POST /v1/account/session: HttpOnly, Secure,\n    SameSite=Strict, Path=/v1/account, 7 days from sign-in. Read-only: it opens no paid route\n    and no route that acts on a key.'\n  sources:\n  - openapi/ibanforge-account-api-openapi.yml\n  - openapi/ibanforge-api-keys-api-openapi.yml\n  - openapi/ibanforge-bic-api-openapi.yml\n  - openapi/ibanforge-compliance-api-openapi.yml\n  - openapi/ibanforge-credits-api-openapi.yml\n  - openapi/ibanforge-free-api-openapi.yml\n  - openapi/ibanforge-iban-api-openapi.yml\n  - openapi/ibanforge-mcp-api-openapi.yml\n  - openapi/ibanforge-swiss-clearing-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/authentication/ibanforge-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Finance
- Banking
- Compliance
- MCP
- A2A
---
