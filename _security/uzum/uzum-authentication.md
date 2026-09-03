---
api_key_in:
- header
api_specs:
- filename: uzum-checkout-openapi.yaml
  format: yaml
  label: Uzum Checkout
  slug: uzum-checkout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-checkout-openapi.yaml
- filename: uzum-crossborder-openapi.yaml
  format: yaml
  label: Uzum CrossBorder Transfer
  slug: uzum-crossborder-transfer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-crossborder-openapi.yaml
- filename: uzum-remitcore-openapi.yaml
  format: yaml
  label: Remit Core
  slug: uzum-remit-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-remitcore-openapi.yaml
- filename: uzum-nasiya-openapi.yaml
  format: yaml
  label: Uzum Nasiya Partner API
  slug: uzum-nasiya-partner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-nasiya-openapi.yaml
- filename: uzum-fiscalization-openapi.yaml
  format: yaml
  label: Uzum Fiscalization
  slug: uzum-fiscalization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-fiscalization-openapi.yaml
- filename: uzum-fastpay-openapi.yaml
  format: yaml
  label: Uzum Fast Pay
  slug: uzum-fast-pay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-fastpay-openapi.yaml
- filename: uzum-dynamicqr-openapi.yaml
  format: yaml
  label: Uzum Dynamic QR
  slug: uzum-dynamic-qr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-dynamicqr-openapi.yaml
- filename: uzum-merchant-openapi.yaml
  format: yaml
  label: Uzum Merchant API
  slug: uzum-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-merchant-openapi.yaml
- filename: uzum-ratekeeper-openapi.yaml
  format: yaml
  label: Uzum RateKeeper
  slug: uzum-ratekeeper
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-ratekeeper-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Uzum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uzum secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Uzum
provider_slug: uzum
scheme_count: 3
schemes:
- apis:
  - Uzum CrossBorder Transfer
  - Uzum Merchant API
  - Uzum BaaS Payment Hub
  docs: https://developer.uzumbank.uz/en/paymenthub/auth/
  name: basicAuth
  note: 'Login and password issued per partner, base64-encoded into `Authorization: Basic`. Payment Hub additionally requires Content-Type: application/json and Accept-Language (EN/RU/UZ) and states TLS 1.2 for transport.'
  scheme: basic
  sources:
  - openapi/uzum-crossborder-openapi.yaml
  - openapi/uzum-merchant-openapi.yaml
  type: http
- apis:
  - Uzum Nasiya Partner API
  bearerFormat: JWT
  name: BearerAuth
  note: '`Authorization: Bearer <token>` on every request.'
  scheme: bearer
  sources:
  - openapi/uzum-nasiya-openapi.yaml
  type: http
- apis:
  - Remit Core
  description: Partner API key in UUID format. Issued upon onboarding. Required for all methods
  in: header
  name: XApiKeyAuth
  note: Production access additionally requires an IPSec tunnel and IP allow-listing; the internet-reachable host is the test environment only.
  parameter: X-Api-Key
  sources:
  - openapi/uzum-remitcore-openapi.yaml
  type: apiKey
slug: uzum-authentication
source_filename: uzum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://developer.uzumbank.uz/en/ (per-product Authentication sections) + openapi/ securitySchemes\ndocs: https://developer.uzumbank.uz/en/\nnote: >-\n  Derived from the four specs that declare a securitySchemes block, then upgraded from the\n  Authentication section published in each product's own OpenAPI info.description on\n  developer.uzumbank.uz. Five of the nine contracts (Checkout, Fast Pay, Dynamic QR,\n  Fiscalization, RateKeeper) document their credential model in prose but never declare a\n  securityScheme in the spec, so an agent reading only the machine-readable contract cannot\n  see how to authenticate. That gap is recorded below per API.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  self_service: false\n  credential_issuance: >-\n    Every Uzum Bank API credential is issued by an Uzum account manager after a commercial\n\
  \    agreement. There is no self-service key generation on any surface.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/uzum-crossborder-openapi.yaml\n  - openapi/uzum-merchant-openapi.yaml\n  apis:\n  - Uzum CrossBorder Transfer\n  - Uzum Merchant API\n  - Uzum BaaS Payment Hub\n  note: >-\n    Login and password issued per partner, base64-encoded into `Authorization: Basic`.\n    Payment Hub additionally requires Content-Type: application/json and Accept-Language\n    (EN/RU/UZ) and states TLS 1.2 for transport.\n  docs: https://developer.uzumbank.uz/en/paymenthub/auth/\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/uzum-nasiya-openapi.yaml\n  apis:\n  - Uzum Nasiya Partner API\n  note: '`Authorization: Bearer <token>` on every request.'\n- name: XApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Partner API key in UUID format. Issued upon onboarding. Required for all\
  \ methods\n  sources:\n  - openapi/uzum-remitcore-openapi.yaml\n  apis:\n  - Remit Core\n  note: >-\n    Production access additionally requires an IPSec tunnel and IP allow-listing; the\n    internet-reachable host is the test environment only.\nundeclared_in_spec:\n- api: Uzum Checkout\n  spec: openapi/uzum-checkout-openapi.yaml\n  documented_scheme: apiKey (two headers)\n  headers:\n  - name: X-Terminal-Id\n    description: Transaction-processing terminal identifier assigned to each partner.\n  - name: X-API-Key\n    description: Unique API key assigned to each partner.\n  - name: Content-Language\n    description: 'Payment-form locale. Enum: ru-RU, uz-UZ, en-EN.'\n  source: https://developer.uzumbank.uz/en/checkout\n  gap: securitySchemes absent from the OpenAPI; documented only in info.description.\n- api: Uzum Fast Pay\n  spec: openapi/uzum-fastpay-openapi.yaml\n  documented_scheme: signed header\n  headers:\n  - name: Authorization\n    description: >-\n      Composite signed value\
  \ matching regex ^\\d*:(\\d{40}):\\d*$ — merchant_id, a 40-character\n      hash, and a millisecond timestamp. Requests are rejected (error 403) when more than 50\n      seconds elapse between signing and processing, so the signature is time-bound.\n  source: https://developer.uzumbank.uz/en/fastpay\n  gap: securitySchemes absent from the OpenAPI.\n- api: Uzum Dynamic QR\n  spec: openapi/uzum-dynamicqr-openapi.yaml\n  documented_scheme: signed header (same construction as Fast Pay)\n  source: https://developer.uzumbank.uz/en/dynamicqr\n  gap: securitySchemes absent from the OpenAPI.\n- api: Uzum Fiscalization\n  spec: openapi/uzum-fiscalization-openapi.yaml\n  documented_scheme: apiKey\n  headers:\n  - name: API Key\n    description: >-\n      Unique identifier generated and provided by the Uzum development team per partner.\n      Separate keys are issued for the test and production hosts.\n  source: https://developer.uzumbank.uz/en/fiscalization\n  gap: securitySchemes absent from the\
  \ OpenAPI.\n- api: Uzum RateKeeper\n  spec: openapi/uzum-ratekeeper-openapi.yaml\n  documented_scheme: unknown\n  gap: >-\n    The spec declares no securitySchemes and carries no info.description; the portal page\n    publishes no authentication section for this product.\n- api: Uzum Market Seller API\n  documented_scheme: bearer token issued in the seller cabinet\n  source: https://api-seller.uzum.uz/swagger-ui/index.html\n  gap: >-\n    Anonymous requests return 403 \"RBAC: access denied\" and the Swagger UI 302s to a\n    Keycloak realm (auth.infra.cluster.daymarket.uz, realm `umarket`, client\n    `platform-client-prod`). No public contract or auth reference is served.\noauth:\n  present: false\n  note: >-\n    No OAuth 2.0 or OpenID Connect surface is exposed to partners on any documented Uzum\n    Bank API. The only OIDC deployment observed is the internal Keycloak realm fronting the\n    Uzum Market seller cabinet, which is not a partner authorization surface. scopes/ is\n    therefore\
  \ not applicable and no OAuthScopes artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/authentication/uzum-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Payments
- Banking
- Financial Services
- E-Commerce
- Marketplace
- Money Transfer
- Remittances
- BNPL
- Acquiring
- QR Payments
- Fiscalization
- Banking as a Service
- Uzbekistan
- Central Asia
---
