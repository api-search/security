---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: woolworths-group-accountstatusinquiry-api-openapi.yml
  format: yaml
  label: Woolworths Group Account Status Inquiry API
  slug: woolworths-group-accountstatusinquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-accountstatusinquiry-api-openapi.yml
- filename: woolworths-group-activating-physical-gift-cards-api-openapi.yml
  format: yaml
  label: Woolworths Group Activating Physical Gift Cards API
  slug: woolworths-group-activating-physical-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-activating-physical-gift-cards-api-openapi.yml
- filename: woolworths-group-authorization-api-openapi.yml
  format: yaml
  label: Woolworths Group Authorization API
  slug: woolworths-group-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-authorization-api-openapi.yml
- filename: woolworths-group-capture-api-openapi.yml
  format: yaml
  label: Woolworths Group Capture API
  slug: woolworths-group-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-capture-api-openapi.yml
- filename: woolworths-group-gifting-catalogue-api-openapi.yml
  format: yaml
  label: Woolworths Group Gifting Catalogue API
  slug: woolworths-group-gifting-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-gifting-catalogue-api-openapi.yml
- filename: woolworths-group-health-check-api-openapi.yml
  format: yaml
  label: Woolworths Group Health check API
  slug: woolworths-group-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-health-check-api-openapi.yml
- filename: woolworths-group-instruments-api-openapi.yml
  format: yaml
  label: Woolworths Group Instruments API
  slug: woolworths-group-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-instruments-api-openapi.yml
- filename: woolworths-group-key-management-api-openapi.yml
  format: yaml
  label: Woolworths Group Key Management API
  slug: woolworths-group-key-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-key-management-api-openapi.yml
- filename: woolworths-group-order-api-openapi.yml
  format: yaml
  label: Woolworths Group Order API
  slug: woolworths-group-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-order-api-openapi.yml
- filename: woolworths-group-ordering-digital-gift-cards-api-openapi.yml
  format: yaml
  label: Woolworths Group Ordering Digital Gift Cards API
  slug: woolworths-group-ordering-digital-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-ordering-digital-gift-cards-api-openapi.yml
- filename: woolworths-group-payments-api-openapi.yml
  format: yaml
  label: Woolworths Group Payments API
  slug: woolworths-group-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-payments-api-openapi.yml
- filename: woolworths-group-refund-api-openapi.yml
  format: yaml
  label: Woolworths Group Refund API
  slug: woolworths-group-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-refund-api-openapi.yml
- filename: woolworths-group-refunds-api-openapi.yml
  format: yaml
  label: Woolworths Group Refunds API
  slug: woolworths-group-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-refunds-api-openapi.yml
- filename: woolworths-group-support-api-openapi.yml
  format: yaml
  label: Woolworths Group Support API
  slug: woolworths-group-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-support-api-openapi.yml
- filename: woolworths-group-transaction-api-openapi.yml
  format: yaml
  label: Woolworths Group Transaction API
  slug: woolworths-group-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-transaction-api-openapi.yml
- filename: woolworths-group-void-api-openapi.yml
  format: yaml
  label: Woolworths Group Void API
  slug: woolworths-group-void-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-void-api-openapi.yml
- filename: woolworths-group-wallet-services-api-openapi.yml
  format: yaml
  label: Woolworths Group Wallet Services API
  slug: woolworths-group-wallet-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-wallet-services-api-openapi.yml
auth_types:
- apiKey
- http
- signed-request
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Woolworths Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Woolworths Group secures its APIs with apiKey, http, and signed-request across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Woolworths Group
provider_slug: woolworths-group
scheme_count: 5
schemes:
- applies_to: Wpay Gift Card Partner API
  description: Partner integration key. Wpay issues a test-environment key at onboarding and a production key after certification, and adds the partner's production IP addresses to an allow list before go-live.
  in: header
  name: X-Api-Key
  parameter: X-Api-Key
  sources:
  - openapi/woolworths-group-wpay-gift-card-partner-openapi.yml
  - https://developerhub.wpay.com.au/giftingservices/docs/becoming-a-gifting-partner
  type: apiKey
- applies_to: Wpay Gifting Client API
  bearerFormat: JWT
  description: The client generates an ES256 (prime256v1) key pair and gives Wpay its public key, Key ID and IPs to whitelist. In return Wpay issues an apiClientId, which goes in the JWT payload. A JWS is sent in the headers of every request.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/woolworths-group-wpay-gifting-client-openapi.yml
  - https://developerhub.wpay.com.au/giftingservices/docs/jwt-authentication-process
  type: http
- applies_to: Wpay Cards Connect (card-not-present) API
  description: The client generates two private/public key pairs in JWK format (Sandbox and Production) and shares the public keys. Every request carries a unique JWT signed into a JWS with method, path, query and sha256 claims, and the server checks those claims against the request (errors AUTH01-AUTH21). Credentials can be rotated by API (PUT /api/v1/keys/credential/rotate-to/{keyId}); a new credential's expiration cannot be more than 365 days in the future.
  name: cards-connect-jws
  scheme: JWS (signed request)
  sources:
  - https://developerhub.wpay.com.au/cardsconnect/docs/authentication
  - https://developerhub.wpay.com.au/cardsconnect/docs/credential-rotation
  - https://developerhub.wpay.com.au/cardsconnect/docs/error-codes
  type: http
- applies_to: Wpay Cards Connect in-store (Connextor) API
  description: Requests are signed with X-Authorization (wpay-http-hmac id/nonce/version/headers/signature, version connextor-1.0), X-Authorization-Timestamp (rejected if it differs from server time by more than 900 seconds) and X-Authorization-Content-SHA256. The server signs responses with X-Server-Authorization-HMAC-SHA256.
  name: connextor-http-hmac
  parameters:
  - X-Authorization
  - X-Authorization-Timestamp
  - X-Authorization-Content-SHA256
  scheme: wpay-http-hmac (HMAC-SHA256)
  sources:
  - openapi/woolworths-group-wpay-payment-openapi.yml
  - openapi/_original/wpay-developerhub/cardsconnect__overview-of-headers.md
  - openapi/_original/wpay-developerhub/cardsconnect__generating-the-client-request-header-and-signature.md
  type: http
- applies_to: Wpay NPP PayTo Merchant API
  description: The merchant is onboarded with a merchantId GUID, provides a public key and receives a Key ID (kid). Each request is signed as an ES256 JWS whose payload holds method, path, query, sha256 (of the body), iat and exp; exp must be within 60 seconds of iat.
  header: 'Authorization: JWS <JWStoken>'
  name: payto-jws
  scheme: JWS
  sources:
  - https://developerhub.wpay.com.au/payto/docs/getting-connected
  - https://developerhub.wpay.com.au/payto/docs/signing-api-requests
  type: http
slug: woolworths-group-authentication
source_filename: woolworths-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://developerhub.wpay.com.au/giftingservices/docs/jwt-authentication-process\ndocs: https://developerhub.wpay.com.au/giftingservices/docs/jwt-authentication-process\nsummary:\n  types:\n  - apiKey\n  - http\n  - signed-request\n  api_key_in:\n  - header\n  note: Wpay publishes a different auth scheme per product. Only the two gifting specs declare securitySchemes; the Cards Connect, Connextor in-store and PayTo specs declare none, so their schemes below\n    come from the docs.\nschemes:\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  applies_to: Wpay Gift Card Partner API\n  description: Partner integration key. Wpay issues a test-environment key at onboarding and a production key after certification, and adds the partner's production IP addresses to an allow list before\n    go-live.\n  sources:\n  - openapi/woolworths-group-wpay-gift-card-partner-openapi.yml\n  - https://developerhub.wpay.com.au/giftingservices/docs/becoming-a-gifting-partner\n\
  - name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: Wpay Gifting Client API\n  description: The client generates an ES256 (prime256v1) key pair and gives Wpay its public key, Key ID and IPs to whitelist. In return Wpay issues an apiClientId, which goes in the JWT payload. A JWS\n    is sent in the headers of every request.\n  sources:\n  - openapi/woolworths-group-wpay-gifting-client-openapi.yml\n  - https://developerhub.wpay.com.au/giftingservices/docs/jwt-authentication-process\n- name: cards-connect-jws\n  type: http\n  scheme: JWS (signed request)\n  applies_to: Wpay Cards Connect (card-not-present) API\n  description: The client generates two private/public key pairs in JWK format (Sandbox and Production) and shares the public keys. Every request carries a unique JWT signed into a JWS with method, path,\n    query and sha256 claims, and the server checks those claims against the request (errors AUTH01-AUTH21). Credentials can be rotated by API (PUT\
  \ /api/v1/keys/credential/rotate-to/{keyId}); a new credential's\n    expiration cannot be more than 365 days in the future.\n  sources:\n  - https://developerhub.wpay.com.au/cardsconnect/docs/authentication\n  - https://developerhub.wpay.com.au/cardsconnect/docs/credential-rotation\n  - https://developerhub.wpay.com.au/cardsconnect/docs/error-codes\n- name: connextor-http-hmac\n  type: http\n  scheme: wpay-http-hmac (HMAC-SHA256)\n  applies_to: Wpay Cards Connect in-store (Connextor) API\n  description: Requests are signed with X-Authorization (wpay-http-hmac id/nonce/version/headers/signature, version connextor-1.0), X-Authorization-Timestamp (rejected if it differs from server time by\n    more than 900 seconds) and X-Authorization-Content-SHA256. The server signs responses with X-Server-Authorization-HMAC-SHA256.\n  parameters:\n  - X-Authorization\n  - X-Authorization-Timestamp\n  - X-Authorization-Content-SHA256\n  sources:\n  - openapi/woolworths-group-wpay-payment-openapi.yml\n\
  \  - openapi/_original/wpay-developerhub/cardsconnect__overview-of-headers.md\n  - openapi/_original/wpay-developerhub/cardsconnect__generating-the-client-request-header-and-signature.md\n- name: payto-jws\n  type: http\n  scheme: JWS\n  header: 'Authorization: JWS <JWStoken>'\n  applies_to: Wpay NPP PayTo Merchant API\n  description: The merchant is onboarded with a merchantId GUID, provides a public key and receives a Key ID (kid). Each request is signed as an ES256 JWS whose payload holds method, path, query, sha256\n    (of the body), iat and exp; exp must be within 60 seconds of iat.\n  sources:\n  - https://developerhub.wpay.com.au/payto/docs/getting-connected\n  - https://developerhub.wpay.com.au/payto/docs/signing-api-requests\ndocs_pages:\n- https://developerhub.wpay.com.au/giftingservices/docs/jwt-authentication-process\n- https://developerhub.wpay.com.au/giftingservices/docs/becoming-a-gifting-partner\n- https://developerhub.wpay.com.au/cardsconnect/docs/authentication\n- https://developerhub.wpay.com.au/cardsconnect/docs/credential-rotation\n\
  - https://developerhub.wpay.com.au/cardsconnect/reference/overview-of-headers\n- https://developerhub.wpay.com.au/payto/docs/getting-connected\n- https://developerhub.wpay.com.au/payto/docs/signing-api-requests\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/authentication/woolworths-group-authentication.yml
summary_line: apiKey/http/signed-request · 5 schemes
tags:
- Company
- Retail
- Supermarkets
- Grocery
- Australia
- New Zealand
- E-Commerce
---
