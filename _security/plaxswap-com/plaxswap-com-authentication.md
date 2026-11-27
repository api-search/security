---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: plaxswap-com-accounts-api-openapi.yml
  format: yaml
  label: Plaxswap Accounts API
  slug: plaxswap-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-accounts-api-openapi.yml
- filename: plaxswap-com-checkout-api-openapi.yml
  format: yaml
  label: Plaxswap Checkout API
  slug: plaxswap-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-checkout-api-openapi.yml
- filename: plaxswap-com-merchant-account-api-openapi.yml
  format: yaml
  label: Plaxswap Merchant account API
  slug: plaxswap-com-merchant-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-merchant-account-api-openapi.yml
- filename: plaxswap-com-orders-api-openapi.yml
  format: yaml
  label: Plaxswap Orders API
  slug: plaxswap-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-orders-api-openapi.yml
- filename: plaxswap-com-partner-portal-api-openapi.yml
  format: yaml
  label: Plaxswap Partner portal API
  slug: plaxswap-com-partner-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-partner-portal-api-openapi.yml
- filename: plaxswap-com-payment-gateway-api-openapi.yml
  format: yaml
  label: Plaxswap Payment gateway API
  slug: plaxswap-com-payment-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-payment-gateway-api-openapi.yml
- filename: plaxswap-com-payment-links-api-openapi.yml
  format: yaml
  label: Plaxswap Payment links API
  slug: plaxswap-com-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-payment-links-api-openapi.yml
- filename: plaxswap-com-price-alerts-api-openapi.yml
  format: yaml
  label: Plaxswap Price alerts API
  slug: plaxswap-com-price-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-price-alerts-api-openapi.yml
- filename: plaxswap-com-sandbox-api-openapi.yml
  format: yaml
  label: Plaxswap Sandbox API
  slug: plaxswap-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-sandbox-api-openapi.yml
- filename: plaxswap-com-service-api-openapi.yml
  format: yaml
  label: Plaxswap Service API
  slug: plaxswap-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-service-api-openapi.yml
- filename: plaxswap-com-support-api-openapi.yml
  format: yaml
  label: Plaxswap Support API
  slug: plaxswap-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-support-api-openapi.yml
- filename: plaxswap-com-swaps-api-openapi.yml
  format: yaml
  label: Plaxswap Swaps API
  slug: plaxswap-com-swaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-swaps-api-openapi.yml
- filename: plaxswap-com-webhooks-api-openapi.yml
  format: yaml
  label: Plaxswap Webhooks API
  slug: plaxswap-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaxswap-com/openapi/plaxswap-com-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Plaxswap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plaxswap secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Plaxswap
provider_slug: plaxswap-com
scheme_count: 4
schemes:
- description: Partner API key, pxk_<prefix>_<secret>. Created in the admin console and shown once. A wrong or switched-off key gets 401 invalid_api_key.
  in: header
  name: partnerKey
  parameter: x-api-key
  sources:
  - openapi/plaxswap-com-openapi.json
  type: apiKey
- description: 'The same API key as Authorization: Bearer pxk_<prefix>_<secret>.'
  name: partnerBearer
  scheme: bearer
  sources:
  - openapi/plaxswap-com-openapi.json
  type: http
- description: 'Merchant owner session after Google or Telegram login. Writes also require x-px-merchant: 1 and the site Origin. API keys cannot manage accounts, credentials or withdrawals.'
  in: cookie
  name: merchantCookie
  parameter: px_merchant
  sources:
  - openapi/plaxswap-com-openapi.json
  type: apiKey
- description: The browser's account key (HttpOnly). Set by POST /api/v1/account or /api/v1/account/restore.
  in: cookie
  name: accountCookie
  parameter: px_acct
  sources:
  - openapi/plaxswap-com-openapi.json
  type: apiKey
slug: plaxswap-com-authentication
source_filename: plaxswap-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/plaxswap-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: partnerKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Partner API key, pxk_<prefix>_<secret>. Created in the admin console and shown\n    once. A wrong or switched-off key gets 401 invalid_api_key.\n  sources:\n  - openapi/plaxswap-com-openapi.json\n- name: partnerBearer\n  type: http\n  scheme: bearer\n  description: 'The same API key as Authorization: Bearer pxk_<prefix>_<secret>.'\n  sources:\n  - openapi/plaxswap-com-openapi.json\n- name: merchantCookie\n  type: apiKey\n  in: cookie\n  parameter: px_merchant\n  description: 'Merchant owner session after Google or Telegram login. Writes also require x-px-merchant:\n    1 and the site Origin. API keys cannot manage accounts, credentials or withdrawals.'\n  sources:\n  - openapi/plaxswap-com-openapi.json\n- name: accountCookie\n\
  \  type: apiKey\n  in: cookie\n  parameter: px_acct\n  description: The browser's account key (HttpOnly). Set by POST /api/v1/account or /api/v1/account/restore.\n  sources:\n  - openapi/plaxswap-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/plaxswap-com/authentication/plaxswap-com-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Cryptocurrency
- Payments
- Wallets
- Swap
---
