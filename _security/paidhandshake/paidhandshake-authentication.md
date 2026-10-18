---
anonymous_access: false
api_key_in: []
api_specs:
- filename: paidhandshake-capabilities-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Capabilities API
  slug: paidhandshake-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-capabilities-api-openapi.yml
- filename: paidhandshake-checkout-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Checkout API
  slug: paidhandshake-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-checkout-api-openapi.yml
- filename: paidhandshake-inventory-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Inventory API
  slug: paidhandshake-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-inventory-api-openapi.yml
- filename: paidhandshake-machine-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Machine API
  slug: paidhandshake-machine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-machine-api-openapi.yml
- filename: paidhandshake-proof-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Proof API
  slug: paidhandshake-proof-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-proof-api-openapi.yml
- filename: paidhandshake-quote-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Quote API
  slug: paidhandshake-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-quote-api-openapi.yml
- filename: paidhandshake-sample-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Sample API
  slug: paidhandshake-sample-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-sample-api-openapi.yml
- filename: paidhandshake-search-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange Search API
  slug: paidhandshake-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-search-api-openapi.yml
- filename: paidhandshake-well-known-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange .well Known API
  slug: paidhandshake-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-well-known-api-openapi.yml
- filename: paidhandshake-x402-api-openapi.yml
  format: yaml
  label: PaidHandshake Exchange X402 API
  slug: paidhandshake-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/openapi/paidhandshake-x402-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Paidhandshake Authentication
name_suffix: Authentication
oauth_flows: []
overview: PaidHandshake Exchange secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PaidHandshake Exchange
provider_slug: paidhandshake
scheme_count: 1
schemes:
- description: One-time-issued phm_ machine API key. Store securely; PaidHandshake stores only a hash.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paidhandshake-openapi.json
  type: http
slug: paidhandshake-authentication
source_filename: paidhandshake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: derived\nsource: openapi/paidhandshake-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: One-time-issued phm_ machine API key. Store securely; PaidHandshake stores only\n    a hash.\n  sources:\n  - openapi/paidhandshake-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paidhandshake/refs/heads/main/authentication/paidhandshake-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Marketplace
- Data
- Automation
---
