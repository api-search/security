---
api_key_in:
- header
api_specs:
- filename: barogo-areas-api-openapi.yml
  format: yaml
  label: Barogo Areas API
  slug: barogo-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-areas-api-openapi.yml
- filename: barogo-delivery-api-openapi.yml
  format: yaml
  label: Barogo Delivery API
  slug: barogo-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-delivery-api-openapi.yml
- filename: barogo-deposits-api-openapi.yml
  format: yaml
  label: Barogo Deposits API
  slug: barogo-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-deposits-api-openapi.yml
- filename: barogo-orders-api-openapi.yml
  format: yaml
  label: Barogo Orders API
  slug: barogo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-orders-api-openapi.yml
- filename: barogo-stores-api-openapi.yml
  format: yaml
  label: Barogo Stores API
  slug: barogo-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-stores-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Barogo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Barogo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Barogo
provider_slug: barogo
scheme_count: 1
schemes:
- description: 고릴라는 API Key 기반으로 접근 권한을 확인합니다. Gorela authenticates every request with a long-lived API key presented as an HTTP bearer token. There is no OAuth, no OIDC, no token exchange and no refresh flow — the key itself is the credential.
  format: 'Authorization: Bearer {API_Key}'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/barogo-gorela-openapi.yml
  - https://developer.gorelas.com/api-docs-md/index.md
  type: http
slug: barogo-authentication
source_filename: barogo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://developer.gorelas.com/api-docs-md/index.md\ndocs: https://developer.gorelas.com/linkage\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  token_model: static-api-key\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer {API_Key}'\n    description: >-\n      고릴라는 API Key 기반으로 접근 권한을 확인합니다. Gorela authenticates every request with a\n      long-lived API key presented as an HTTP bearer token. There is no OAuth, no OIDC, no\n      token exchange and no refresh flow — the key itself is the credential.\n    sources:\n      - openapi/barogo-gorela-openapi.yml\n      - https://developer.gorelas.com/api-docs-md/index.md\nissuance:\n  process: >-\n    Keys are not self-serve. Onboarding runs: (1) commercial agreement with a Barogo sales /\n    operations owner, (2) sign up on the Gorela\
  \ developer site, (3) register the order-agency\n    entity under 연동 관리 (linkage), (4) issue an API key from that console.\n  console: https://developer.gorelas.com/linkage\n  prerequisite: 제휴 협의 — a signed partner agreement precedes key issuance.\nidentity_fields:\n  - field: orderAgencyId\n    description: The order agency's own identifier inside Gorela; scopes every request and callback.\n  - field: orderAgencyStoreId\n    description: >-\n      The partner's own store key, mapped 1:1 to a Gorela storeId. Store-based operations\n      require this mapping to exist before an order can be accepted.\nfailure_modes:\n  - code: EXPIRED_API_KEY\n    status: 401\n    description: API Key의 유효기간이 만료되었거나, 삭제된 경우 — keys have a validity period and can be revoked.\n  - code: VERIFY_API_KEY_FAIL\n    status: 401\n    description: API Key 검증에 실패한 경우.\n  - code: ROLE_DENY\n    status: 401\n    description: >-\n      권한이 없는 API를 요청한 경우 — keys carry a role. Gorela does enforce per-key authorization,\n\
  \      but it publishes no scope or permission reference, so the role surface is not\n      externally enumerable.\ncallback_authentication:\n  documented: false\n  note: >-\n    The 20 Gorela → partner callbacks are plain POSTs. The published reference documents no\n    signature header, shared secret, mTLS or replay window for inbound callbacks; it offers\n    IP allow-listing on request (고릴라 Outbound) as the only stated control. An integrator\n    should treat callback bodies as unauthenticated and confirm state with a read operation.\n  ip_allowlist_contact: tech_poc@barogo.com\ngaps:\n  - No OAuth 2.0 / OIDC surface, so no delegated authorization and no per-user consent.\n  - No published scope or permission reference, despite a ROLE_DENY error code implying roles exist.\n  - No documented key rotation procedure or key lifetime.\n  - No callback signing scheme published.\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://developer.gorelas.com/api-docs-md/index.md\n  http_status:\
  \ 200\n  content_type: text/markdown; charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/authentication/barogo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Delivery
- Logistics
- Last Mile Delivery
- Food Delivery
- Courier
- Fulfillment
- Order
- Webhook
- South Korea
- Transportation
- Marketplace
---
