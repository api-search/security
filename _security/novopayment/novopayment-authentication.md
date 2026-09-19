---
anonymous_access: false
api_key_in: []
api_specs:
- filename: novopayment-accounts-openapi.yml
  format: yaml
  label: NovoPayment Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-accounts-openapi.yml
- filename: novopayment-alias-directory-openapi.yml
  format: yaml
  label: NovoPayment Alias Directory API
  slug: alias-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-alias-directory-openapi.yml
- filename: novopayment-cards-openapi.yml
  format: yaml
  label: NovoPayment Cards API
  slug: cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-cards-openapi.yml
- filename: novopayment-compliance-openapi.yml
  format: yaml
  label: NovoPayment Compliance API
  slug: compliance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-compliance-openapi.yml
- filename: novopayment-customers-openapi.yml
  format: yaml
  label: NovoPayment Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-customers-openapi.yml
- filename: novopayment-issuer-tokenization-openapi.yml
  format: yaml
  label: NovoPayment Issuer Tokenization API
  slug: issuer-tokenization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-issuer-tokenization-openapi.yml
- filename: novopayment-mastercard-issuer-tokenization-openapi.yml
  format: yaml
  label: NovoPayment MasterCard Tokenization API
  slug: mastercard-issuer-tokenization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-mastercard-issuer-tokenization-openapi.yml
- filename: novopayment-merchant-presented-qr-openapi.yml
  format: yaml
  label: NovoPayment Merchant Presented QR
  slug: merchant-presented-qr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-merchant-presented-qr-openapi.yml
- filename: novopayment-oauth2-data-encryption-openapi.yml
  format: yaml
  label: NovoPayment Security OAuth2 API
  slug: oauth2-data-encryption
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-oauth2-data-encryption-openapi.yml
- filename: novopayment-onboarding-openapi.yml
  format: yaml
  label: NovoPayment Onboarding API
  slug: onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-onboarding-openapi.yml
- filename: novopayment-operations-openapi.yml
  format: yaml
  label: NovoPayment Operations API
  slug: operations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-operations-openapi.yml
- filename: novopayment-payment-authorizer-openapi.yml
  format: yaml
  label: NovoPayment Payment Authorizer API
  slug: payment-authorizer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-payment-authorizer-openapi.yml
- filename: novopayment-profile-openapi.yml
  format: yaml
  label: NovoPayment Profile API
  slug: profile
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-profile-openapi.yml
- filename: novopayment-push-provisioning-openapi.yml
  format: yaml
  label: NovoPayment Push Provisioning API
  slug: push-provisioning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-push-provisioning-openapi.yml
- filename: novopayment-real-time-payments-openapi.yml
  format: yaml
  label: NovoPayment Real-Time Payments API
  slug: real-time-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-real-time-payments-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Novopayment Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: NovoPayment secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: NovoPayment
provider_slug: novopayment
scheme_count: 1
schemes:
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  sources:
  - openapi/novopayment-accounts-openapi.yml
  - openapi/novopayment-alias-directory-openapi.yml
  - openapi/novopayment-cards-openapi.yml
  - openapi/novopayment-compliance-openapi.yml
  - openapi/novopayment-customers-openapi.yml
  - openapi/novopayment-mastercard-issuer-tokenization-openapi.yml
  - openapi/novopayment-merchant-presented-qr-openapi.yml
  - openapi/novopayment-onboarding-openapi.yml
  - openapi/novopayment-operations-openapi.yml
  - openapi/novopayment-profile-openapi.yml
  - openapi/novopayment-push-provisioning-openapi.yml
  - openapi/novopayment-real-time-payments-openapi.yml
  type: oauth2
slug: novopayment-authentication
source_filename: novopayment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/novopayment-accounts-openapi.yml, openapi/novopayment-alias-directory-openapi.yml, openapi/novopayment-cards-openapi.yml,\n  openapi/novopayment-compliance-openapi.yml, openapi/novopayment-customers-openapi.yml, openapi/novopayment-mastercard-issuer-tokenization-openapi.yml,\n  openapi/novopayment-merchant-presented-qr-openapi.yml, openapi/novopayment-onboarding-openapi.yml, openapi/novopayment-operations-openapi.yml,\n  openapi/novopayment-profile-openapi.yml, openapi/novopayment-push-provisioning-openapi.yml, openapi/novopayment-real-time-payments-openapi.yml\n  ; plus the developer hub access-token guide and the Security OAuth2 API reference read 2026-09-17\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n    scopes: 0\n  description:\
  \ See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n  sources:\n  - openapi/novopayment-accounts-openapi.yml\n  - openapi/novopayment-alias-directory-openapi.yml\n  - openapi/novopayment-cards-openapi.yml\n  - openapi/novopayment-compliance-openapi.yml\n  - openapi/novopayment-customers-openapi.yml\n  - openapi/novopayment-mastercard-issuer-tokenization-openapi.yml\n  - openapi/novopayment-merchant-presented-qr-openapi.yml\n  - openapi/novopayment-onboarding-openapi.yml\n  - openapi/novopayment-operations-openapi.yml\n  - openapi/novopayment-profile-openapi.yml\n  - openapi/novopayment-push-provisioning-openapi.yml\n  - openapi/novopayment-real-time-payments-openapi.yml\ndocs:\n- https://developer.novopayment.com/guides/how-it-works/get-access-token\n- https://developer.novopayment.com/api/data-encryption/oauth2-data-encryption-api-v1.0\n- https://developer.novopayment.com/guides/data-encryption\ntoken:\n  endpoint: https://sandbox-api.novopayment.com/oauth2/token\n\
  \  grant_type: client_credentials\n  request_encoding: application/x-www-form-urlencoded\n  token_type: BearerToken\n  expires_in_seconds: 1799\n  credentials: client_id + client_secret issued per project per environment from the developer hub dashboard\n  evidence: POST /token request/response examples in openapi/novopayment-oauth2-data-encryption-openapi.yml\nundeclared_schemes:\n- name: apikey\n  location: query\n  apis:\n  - merchant-presented-qr\n  description: Public API key, distinct from the shared secret. Declared as a required query parameter, not as a\n    securityScheme.\n- name: X-Pay-Token\n  location: header\n  apis:\n  - merchant-presented-qr\n  lifetime_seconds: 480\n  description: Token identifying the transaction and its contents; expires in 480 seconds for all clients.\n- name: X-Tenant-Id\n  location: header\n  apis:\n  - all\n  description: Required tenant identifier on every operation; partitions all data by calling tenant.\ntwo_factor:\n  required_for_portal: true\n\
  \  evidence: The developer hub states two-factor authentication is mandatory for portal accounts.\nscopes:\n  published: false\n  artifact: scopes/novopayment-scopes.yml\nnote: NovoPayment secures the API surface with a single OAuth2 client-credentials scheme and no scopes, so every\n  token a project holds carries the full permission set of the APIs selected for that project. The Merchant Presented\n  QR contract layers an additional apikey query parameter and a short-lived X-Pay-Token header on top, declared\n  as plain parameters rather than securitySchemes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/authentication/novopayment-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Payments
- Banking as a Service
- Embedded Finance
- Card Issuing
- Digital Wallet
- Tokenization
- Real-Time Payments
- Onboarding
- KYC
- Latin America
- Fintech
- Digital Banking
---
