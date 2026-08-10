---
api_key_in:
- header
api_specs:
- filename: chargeafter-accounts-api-openapi.yml
  format: yaml
  label: ChargeAfter Accounts API
  slug: chargeafter-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-accounts-api-openapi.yml
- filename: chargeafter-applicationsv3-api-openapi.yml
  format: yaml
  label: ChargeAfter Applications V3 API
  slug: chargeafter-applicationsv3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-applicationsv3-api-openapi.yml
- filename: chargeafter-charges-api-openapi.yml
  format: yaml
  label: ChargeAfter Charges API
  slug: chargeafter-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-charges-api-openapi.yml
- filename: chargeafter-checkout-api-openapi.yml
  format: yaml
  label: ChargeAfter Checkout API
  slug: chargeafter-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-checkout-api-openapi.yml
- filename: chargeafter-consumer-management-api-openapi.yml
  format: yaml
  label: ChargeAfter Consumer Management API
  slug: chargeafter-consumer-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-consumer-management-api-openapi.yml
- filename: chargeafter-consumersv2-api-openapi.yml
  format: yaml
  label: ChargeAfter Consumers V2 API
  slug: chargeafter-consumersv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-consumersv2-api-openapi.yml
- filename: chargeafter-fundings-api-openapi.yml
  format: yaml
  label: ChargeAfter Fundings API
  slug: chargeafter-fundings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-fundings-api-openapi.yml
- filename: chargeafter-lenders-api-openapi.yml
  format: yaml
  label: ChargeAfter Lenders API
  slug: chargeafter-lenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-lenders-api-openapi.yml
- filename: chargeafter-links-api-openapi.yml
  format: yaml
  label: ChargeAfter Links API
  slug: chargeafter-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-links-api-openapi.yml
- filename: chargeafter-orders-api-openapi.yml
  format: yaml
  label: ChargeAfter Orders API
  slug: chargeafter-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-orders-api-openapi.yml
- filename: chargeafter-sessionsv3-api-openapi.yml
  format: yaml
  label: ChargeAfter Sessions V3 API
  slug: chargeafter-sessionsv3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-sessionsv3-api-openapi.yml
- filename: chargeafter-transactions-api-openapi.yml
  format: yaml
  label: ChargeAfter Transactions API
  slug: chargeafter-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/openapi/chargeafter-transactions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Chargeafter Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChargeAfter secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ChargeAfter
provider_slug: chargeafter
scheme_count: 3
schemes:
- description: 'Declared as an apiKey scheme in the OpenAPI, but the documented wire format is `Authorization: Bearer <PRIVATE_API_KEY>` — the spec models a bearer credential as an apiKey header.'
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/chargeafter-charge-api-openapi.yml
  - openapi/chargeafter-checkout-application-status-openapi.yml
  - openapi/chargeafter-checkout-application-token-openapi.yml
  - openapi/chargeafter-checkout-session-accounts-openapi.yml
  - openapi/chargeafter-checkout-session-openapi.yml
  - openapi/chargeafter-consumer-api-openapi.yml
  - openapi/chargeafter-consumer-credit-lookup-openapi.yml
  - openapi/chargeafter-consumer-details-openapi.yml
  - openapi/chargeafter-disputes-management-lenders-openapi.yml
  - openapi/chargeafter-distribution-api-openapi.yml
  - openapi/chargeafter-funding-api-openapi.yml
  type: apiKey
- description: ChargeAfter API uses bearer authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chargeafter-consumers-management-openapi.yml
  type: http
- bearerFormat: bearerFormat
  description: Capitalized `Bearer` scheme value — a spec defect; RFC 7235 scheme names in OpenAPI `http` schemes are lowercase. Wire behaviour is identical to bearerAuth.
  name: Bearer
  scheme: Bearer
  sources:
  - openapi/chargeafter-omni-link-openapi.yml
  type: http
slug: chargeafter-authentication
source_filename: chargeafter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://docs.chargeafter.com/reference/authentication\ndocs: https://docs.chargeafter.com/reference/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: >-\n    A single static bearer credential sent in the Authorization header. ChargeAfter provisions two keys per\n    environment — a public API key for client-side SDK use and a private API key for server-to-server calls.\n    There is no OAuth 2.0 flow, no token exchange, and no scope surface on the payments API. All requests\n    must be made over HTTPS; a missing, incorrect, or outdated key returns HTTP 401.\ncredentials:\n- name: Public API key\n  usage: client-side\n  description: Used by the ChargeAfter JavaScript SDK in the browser. Safe to expose in public code.\n- name: Private API key\n  usage: server-side\n  description: >-\n    Used for backend REST calls. Must be stored securely on the server and never\
  \ exposed to the client;\n    it performs API requests without restriction.\nenvironments:\n- name: production\n  base_url: https://api.chargeafter.com\n  keys: production key pair\n- name: sandbox\n  base_url: https://api-sandbox.ca-dev.co\n  keys: sandbox key pair\n- name: uat\n  base_url: https://api-uat.ca-dev.co\n  keys: UAT key pair\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Declared as an apiKey scheme in the OpenAPI, but the documented wire format is\n    `Authorization: Bearer <PRIVATE_API_KEY>` — the spec models a bearer credential as an apiKey header.\n  sources:\n  - openapi/chargeafter-charge-api-openapi.yml\n  - openapi/chargeafter-checkout-application-status-openapi.yml\n  - openapi/chargeafter-checkout-application-token-openapi.yml\n  - openapi/chargeafter-checkout-session-accounts-openapi.yml\n  - openapi/chargeafter-checkout-session-openapi.yml\n  - openapi/chargeafter-consumer-api-openapi.yml\n  - openapi/chargeafter-consumer-credit-lookup-openapi.yml\n\
  \  - openapi/chargeafter-consumer-details-openapi.yml\n  - openapi/chargeafter-disputes-management-lenders-openapi.yml\n  - openapi/chargeafter-distribution-api-openapi.yml\n  - openapi/chargeafter-funding-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: ChargeAfter API uses bearer authentication.\n  sources:\n  - openapi/chargeafter-consumers-management-openapi.yml\n- name: Bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: bearerFormat\n  description: >-\n    Capitalized `Bearer` scheme value — a spec defect; RFC 7235 scheme names in OpenAPI `http` schemes are\n    lowercase. Wire behaviour is identical to bearerAuth.\n  sources:\n  - openapi/chargeafter-omni-link-openapi.yml\nnotes:\n- >-\n  Three different security-scheme shapes (`apiKey` in header, `bearerAuth`, `Bearer`) describe one credential\n  across ChargeAfter's twelve published definitions. The apiKey scheme's own description says the key is\n  \"provided in the `apiKey` HTTP header\"\
  , which contradicts both its own `name: Authorization` and the\n  documented `Authorization: Bearer` form.\n- >-\n  A separate OAuth 2.0 authorization server is published on the marketing site at\n  https://chargeafter.com/.well-known/oauth-authorization-server with `scopes_supported: [mcp]`. It fronts a\n  WordPress MCP endpoint, not the payments API — see mcp/chargeafter-mcp.yml.\nx-evidence:\n- url: https://docs.chargeafter.com/reference/authentication\n  http_status: 200\n  fetched: '2026-08-09'\n- url: https://docs.chargeafter.com/reference/api-environments\n  http_status: 200\n  fetched: '2026-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargeafter/refs/heads/main/authentication/chargeafter-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Financial Services
- Payments
- Lending
- Buy Now Pay Later
- Embedded Finance
- Point of Sale
- Ecommerce
- Checkout
- Consumer Credit
- Retail
---
