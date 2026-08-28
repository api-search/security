---
api_key_in: []
api_specs:
- filename: klarna-payments-api-openapi.yml
  format: yaml
  label: Klarna Payments API
  slug: klarna-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payments-api-openapi.yml
- filename: klarna-checkout-api-openapi.yml
  format: yaml
  label: Klarna Checkout API
  slug: klarna-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-checkout-api-openapi.yml
- filename: klarna-customer-token-api-openapi.yml
  format: yaml
  label: Klarna Customer Token API
  slug: klarna-customer-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-customer-token-api-openapi.yml
- filename: klarna-push-notifications-asyncapi.yml
  format: yaml
  label: Klarna Push Notifications
  slug: klarna-push-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/asyncapi/klarna-push-notifications-asyncapi.yml
- filename: klarna-captures-api-openapi.yml
  format: yaml
  label: Klarna Captures API
  slug: klarna-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-captures-api-openapi.yml
- filename: klarna-checkout-api-openapi.yml
  format: yaml
  label: Klarna Checkout API
  slug: klarna-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-checkout-api-openapi.yml
- filename: klarna-customer-token-api-openapi.yml
  format: yaml
  label: Klarna Customer Token API
  slug: klarna-customer-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-customer-token-api-openapi.yml
- filename: klarna-hpp-api-openapi.yml
  format: yaml
  label: Klarna Hpp API
  slug: klarna-hpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-hpp-api-openapi.yml
- filename: klarna-merchant-urls-address-update-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.address Update API
  slug: klarna-merchant-urls-address-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-address-update-api-openapi.yml
- filename: klarna-merchant-urls-country-change-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.country Change API
  slug: klarna-merchant-urls-country-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-country-change-api-openapi.yml
- filename: klarna-merchant-urls-shipping-option-update-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.shipping Option Update API
  slug: klarna-merchant-urls-shipping-option-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-shipping-option-update-api-openapi.yml
- filename: klarna-merchant-urls-validation-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.validation API
  slug: klarna-merchant-urls-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-validation-api-openapi.yml
- filename: klarna-merchantcard-api-openapi.yml
  format: yaml
  label: Klarna Merchantcard API
  slug: klarna-merchantcard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchantcard-api-openapi.yml
- filename: klarna-orders-api-openapi.yml
  format: yaml
  label: Klarna Orders API
  slug: klarna-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-orders-api-openapi.yml
- filename: klarna-payments-api-openapi.yml
  format: yaml
  label: Klarna Payments API
  slug: klarna-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payments-api-openapi.yml
- filename: klarna-payouts-api-openapi.yml
  format: yaml
  label: Klarna Payouts API
  slug: klarna-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payouts-api-openapi.yml
- filename: klarna-refunds-api-openapi.yml
  format: yaml
  label: Klarna Refunds API
  slug: klarna-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-refunds-api-openapi.yml
- filename: klarna-reports-api-openapi.yml
  format: yaml
  label: Klarna Reports API
  slug: klarna-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-reports-api-openapi.yml
- filename: klarna-transactions-api-openapi.yml
  format: yaml
  label: Klarna Transactions API
  slug: klarna-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-transactions-api-openapi.yml
auth_types:
- http
- openIdConnect
description: Klarna runs three distinct authentication surfaces. Server-to-server REST APIs use HTTP Basic with a Klarna-issued API key as the credential. Browser-side libraries (Web SDK, Klarna Payments JS, On-site Messaging) use a non-secret client-id bound to an allow-list of origins. Sign in with Klarna is a full OAuth 2.0 / OpenID Connect authorization-code flow at login.klarna.com. The OpenAPI files in this repo only declare the first of the three.
kind: authentication
layout: security
method: searched
name: Klarna Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Klarna secures its APIs with http and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Klarna
provider_slug: klarna
scheme_count: 4
schemes:
- credential_format: klarna_<live|test>_api_<random>
  environments:
    live_prefix: klarna_live_api_
    test_prefix: klarna_test_api_
  failure: 401 Unauthorized when credentials are missing or incorrect
  header: 'Authorization: Basic <API key>'
  issued_from: Merchant Portal (portal.klarna.com / portal.playground.klarna.com)
  lifecycle: Klarna disables API credentials after two months of inactivity and deletes them after ten months of inactivity. A disabled credential can be reactivated before deletion.
  name: basic_auth
  note: 'Klarna documents the API key as the Basic credential directly — `Authorization: Basic <API key>` — either raw or base64-encoded. Clients that can only send a username/password pair may use the UUID username shown alongside the key in the Merchant Portal: `Authorization: Basic <UUID>:<API key>`. Keys are bound to a Merchant ID (MID); one MID may hold several keys.'
  scheme: basic
  sources:
  - openapi/klarna-settlements-api-openapi.yml
  - openapi/order-management-api-openapi.yml
  type: http
- credential_format: klarna_<live|test>_client_<random>
  in: script-attribute
  name: client_id
  note: Used by the browser-loaded Klarna Web SDK, Klarna Payments JS library and On-site Messaging. Klarna states the client-id is not secret in itself and must be configured with a list of approved websites from which it may be used. Both API keys and client-ids are signed tokens the platform verifies.
  parameter_name: data-client-id
  secret: false
  sources:
  - https://docs.klarna.com/api/kn/direct-partner/security/
  type: apiKey
- flows:
  - authorizationUrl: https://login.klarna.com/oauth2/auth
    flow: authorizationCode
    pkce:
    - S256
    revocationUrl: https://login.klarna.com/oauth2/revoke
    scope_count: 34
    tokenUrl: https://login.klarna.com/oauth2/token
    userinfoUrl: https://login.klarna.com/userinfo
  issuer: https://login.klarna.com
  name: SignInWithKlarna
  note: Klarna's own security page states Sign in with Klarna authenticates with "OAuth using client-id and API-key". The discovery document supports client_secret_post, client_secret_basic, private_key_jwt and none for token-endpoint auth, and requires PKCE S256.
  openIdConnectUrl: https://login.klarna.com/.well-known/openid-configuration
  scopes_artifact: scopes/klarna-scopes.yml
  sources:
  - https://login.klarna.com/.well-known/openid-configuration
  type: openIdConnect
- name: eIDAS-mTLS
  note: The XS2A API at xs2a.banking.klarna.com is protected with mutual TLS and requires a valid eIDAS certificate from an approved Trust Centre. Klarna validates the certificate and extracts the TPP roles (AIS, PIS, PIIS); an invalid certificate or insufficient role returns 403. Production access additionally requires a PSD2 TPP licence.
  scope: Klarna XS2A (PSD2 open banking) API only
  sources:
  - https://docs.klarna.com/api/xs2a/authentication/
  - https://docs.klarna.com/api/xs2a/requirements/
  type: mutualTLS
slug: klarna-authentication
source_filename: klarna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/klarna-settlements-api-openapi.yml, openapi/order-management-api-openapi.yml\ndocs: https://docs.klarna.com/acquirer/klarna/get-started/integration-resilience/authentication/\ndocs_additional:\n  - https://docs.klarna.com/api/kn/direct-partner/security/\n  - https://login.klarna.com/.well-known/openid-configuration\ndescription: >-\n  Klarna runs three distinct authentication surfaces. Server-to-server REST APIs use HTTP Basic\n  with a Klarna-issued API key as the credential. Browser-side libraries (Web SDK, Klarna Payments\n  JS, On-site Messaging) use a non-secret client-id bound to an allow-list of origins. Sign in with\n  Klarna is a full OAuth 2.0 / OpenID Connect authorization-code flow at login.klarna.com. The\n  OpenAPI files in this repo only declare the first of the three.\nsummary:\n  types:\n    - http\n    - openIdConnect\n  http_schemes:\n    - basic\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n\
  schemes:\n  - name: basic_auth\n    type: http\n    scheme: basic\n    sources:\n      - openapi/klarna-settlements-api-openapi.yml\n      - openapi/order-management-api-openapi.yml\n    credential_format: \"klarna_<live|test>_api_<random>\"\n    header: \"Authorization: Basic <API key>\"\n    note: >-\n      Klarna documents the API key as the Basic credential directly — `Authorization: Basic <API key>`\n      — either raw or base64-encoded. Clients that can only send a username/password pair may use the\n      UUID username shown alongside the key in the Merchant Portal:\n      `Authorization: Basic <UUID>:<API key>`. Keys are bound to a Merchant ID (MID); one MID may hold\n      several keys.\n    environments:\n      live_prefix: klarna_live_api_\n      test_prefix: klarna_test_api_\n    failure: 401 Unauthorized when credentials are missing or incorrect\n    lifecycle: >-\n      Klarna disables API credentials after two months of inactivity and deletes them after ten\n      months\
  \ of inactivity. A disabled credential can be reactivated before deletion.\n    issued_from: Merchant Portal (portal.klarna.com / portal.playground.klarna.com)\n  - name: client_id\n    type: apiKey\n    in: script-attribute\n    parameter_name: data-client-id\n    sources:\n      - https://docs.klarna.com/api/kn/direct-partner/security/\n    credential_format: \"klarna_<live|test>_client_<random>\"\n    secret: false\n    note: >-\n      Used by the browser-loaded Klarna Web SDK, Klarna Payments JS library and On-site Messaging.\n      Klarna states the client-id is not secret in itself and must be configured with a list of\n      approved websites from which it may be used. Both API keys and client-ids are signed tokens\n      the platform verifies.\n  - name: SignInWithKlarna\n    type: openIdConnect\n    openIdConnectUrl: https://login.klarna.com/.well-known/openid-configuration\n    sources:\n      - https://login.klarna.com/.well-known/openid-configuration\n    issuer: https://login.klarna.com\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.klarna.com/oauth2/auth\n        tokenUrl: https://login.klarna.com/oauth2/token\n        revocationUrl: https://login.klarna.com/oauth2/revoke\n        userinfoUrl: https://login.klarna.com/userinfo\n        pkce: [S256]\n        scope_count: 34\n    scopes_artifact: scopes/klarna-scopes.yml\n    note: >-\n      Klarna's own security page states Sign in with Klarna authenticates with \"OAuth using client-id\n      and API-key\". The discovery document supports client_secret_post, client_secret_basic,\n      private_key_jwt and none for token-endpoint auth, and requires PKCE S256.\n  - name: eIDAS-mTLS\n    type: mutualTLS\n    scope: Klarna XS2A (PSD2 open banking) API only\n    sources:\n      - https://docs.klarna.com/api/xs2a/authentication/\n      - https://docs.klarna.com/api/xs2a/requirements/\n    note: >-\n      The XS2A API at xs2a.banking.klarna.com is protected with mutual TLS and requires\
  \ a valid\n      eIDAS certificate from an approved Trust Centre. Klarna validates the certificate and extracts\n      the TPP roles (AIS, PIS, PIIS); an invalid certificate or insufficient role returns 403.\n      Production access additionally requires a PSD2 TPP licence.\ntransport:\n  tls_minimum: TLS 1.2\n  sni_required: true\n  note: >-\n    Klarna requires Server Name Indication in the TLS handshake. Certificates at the API endpoints\n    are issued by AWS Certificate Manager and rotate automatically; Klarna advises pinning the root\n    CA rather than specific certificate details.\nnot_supported:\n  - >-\n    No OAuth 2.0 client-credentials flow for the merchant REST APIs. Machine-to-machine calls to\n    Payments, Order Management, Settlements, Customer Token and HPP are API-key Basic auth only.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/authentication/klarna-authentication.yml
summary_line: http/openIdConnect · 4 schemes
tags:
- Fintech
- BNPL
- Payments
- Cards
- Shopping
- Banking
- Checkout
- Order Management
- Settlement
- Open Banking
- PSD2
- Consumer Credit
- Sweden
---
