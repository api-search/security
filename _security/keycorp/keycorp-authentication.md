---
api_key_in: []
api_specs:
- filename: keycorp-commercial-accounts-reporting-openapi.yml
  format: yaml
  label: KeyBank Account Information API
  slug: account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-commercial-accounts-reporting-openapi.yml
- filename: keycorp-ach-originations-openapi.yml
  format: yaml
  label: KeyBank ACH Origination API
  slug: ach-origination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-ach-originations-openapi.yml
- filename: keycorp-rtp-wire-payments-openapi.yml
  format: yaml
  label: KeyBank Wire Transfer API
  slug: wire-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-rtp-wire-payments-openapi.yml
- filename: keycorp-rtp-wire-payments-openapi.yml
  format: yaml
  label: KeyBank RTP Send Payment API
  slug: rtp-send-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-rtp-wire-payments-openapi.yml
- filename: keycorp-account-validation-openapi.yml
  format: yaml
  label: KeyBank Account Validation API
  slug: account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-account-validation-openapi.yml
- filename: keycorp-ach-inquiry-openapi.yml
  format: yaml
  label: KeyBank ACH Inquiry API
  slug: ach-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-ach-inquiry-openapi.yml
- filename: keycorp-wire-inquiry-openapi.yml
  format: yaml
  label: KeyBank Wire Inquiry API
  slug: wire-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-wire-inquiry-openapi.yml
- filename: keycorp-rtp-inquiry-openapi.yml
  format: yaml
  label: KeyBank RTP Inquiry API
  slug: rtp-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-rtp-inquiry-openapi.yml
- filename: keycorp-check-services-openapi.yml
  format: yaml
  label: KeyBank Check Services API
  slug: check-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-check-services-openapi.yml
- filename: keycorp-webhooks-openapi.yml
  format: yaml
  label: KeyBank Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-webhooks-openapi.yml
auth_types:
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Keycorp Authentication
name_suffix: Authentication
oauth_flows: []
overview: KeyCorp secures its APIs with http and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: KeyCorp
provider_slug: keycorp
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'OAuth2-issued access token supplied in the `Authorization` header using the `Bearer` scheme (e.g. `Authorization: Bearer {token}`). Tokens are minted through KeyBank''s partner OAuth flow (F5 APM); every commercial/embedded banking operation requires a valid bearer token.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/keycorp-account-validation-openapi.yml
  - openapi/keycorp-ach-inquiry-openapi.yml
  - openapi/keycorp-ach-originations-openapi.yml
  - openapi/keycorp-check-services-openapi.yml
  - openapi/keycorp-rtp-inquiry-openapi.yml
  - openapi/keycorp-rtp-wire-payments-openapi.yml
  - openapi/keycorp-wire-inquiry-openapi.yml
  type: http
- description: In addition to the bearer token, all calls to https://partner-api.key.com (and the QV sandbox at https://partner-api-qv.key.com) are transport-secured with a KeyBank-issued mutual-TLS client certificate. Documented as a hard requirement across the KeyBank Developer Portal API catalog.
  name: mutualTLS
  sources:
  - https://developer.key.com/
  type: mutualTLS
slug: keycorp-authentication
source_filename: keycorp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: derived\nsource: openapi/ (KeyBank commercial-banking specs) + developer.key.com\nsummary:\n  types:\n  - http\n  - mutualTLS\n  http_schemes:\n  - bearer\n  bearer_formats:\n  - JWT\n  transport_security:\n  - mutual-TLS (client certificate)\n  additional_headers:\n  - x-fapi-interaction-id\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    OAuth2-issued access token supplied in the `Authorization` header using the\n    `Bearer` scheme (e.g. `Authorization: Bearer {token}`). Tokens are minted\n    through KeyBank's partner OAuth flow (F5 APM); every commercial/embedded\n    banking operation requires a valid bearer token.\n  sources:\n  - openapi/keycorp-account-validation-openapi.yml\n  - openapi/keycorp-ach-inquiry-openapi.yml\n  - openapi/keycorp-ach-originations-openapi.yml\n  - openapi/keycorp-check-services-openapi.yml\n  - openapi/keycorp-rtp-inquiry-openapi.yml\n  - openapi/keycorp-rtp-wire-payments-openapi.yml\n\
  \  - openapi/keycorp-wire-inquiry-openapi.yml\n- name: mutualTLS\n  type: mutualTLS\n  description: >-\n    In addition to the bearer token, all calls to https://partner-api.key.com\n    (and the QV sandbox at https://partner-api-qv.key.com) are transport-secured\n    with a KeyBank-issued mutual-TLS client certificate. Documented as a hard\n    requirement across the KeyBank Developer Portal API catalog.\n  sources:\n  - https://developer.key.com/\nextra:\n  interaction_id:\n    header: x-fapi-interaction-id\n    format: UUID\n    description: >-\n      FAPI-style client-supplied correlation UUID required on request and echoed\n      back on responses for end-to-end traceability. A malformed value returns\n      \"Required header 'x-fapi-interaction-id' is not valid.\"\n  account_context:\n    header: secondaryId\n    description: >-\n      KeyBank-issued secondary identifier required by Account Validation and\n      certain reporting operations to scope the caller to a client relationship.\n\
  notes: >-\n  No OAuth2 securityScheme with scopes is declared in the specs — tokens are\n  opaque-to-consumer bearer JWTs issued out of band, so there is no public OAuth\n  scope surface to catalog (scopes/ is correctly skipped for this provider).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/authentication/keycorp-authentication.yml
summary_line: http/mutualTLS · 2 schemes
tags:
- Banking
- Commercial Banking
- Financial-Services
- Fortune 500
- Payments
- United States
- Super-Regional Bank
- Treasury Management
- Embedded Banking
- ACH
- Real-Time Payments
- Wire Transfer
---
