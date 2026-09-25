---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bbandt-corp-account-information-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Account Information API
  slug: bbandt-corp-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-account-information-api-openapi.yml
- filename: bbandt-corp-account-transactions-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Account Transactions API
  slug: bbandt-corp-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-account-transactions-api-openapi.yml
- filename: bbandt-corp-commercial-account-balance-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Commercial Account Balance API
  slug: bbandt-corp-commercial-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-account-balance-api-openapi.yml
- filename: bbandt-corp-commercial-account-transactions-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Commercial Account Transactions API
  slug: bbandt-corp-commercial-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-account-transactions-api-openapi.yml
- filename: bbandt-corp-commercial-accounts-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Commercial Accounts API
  slug: bbandt-corp-commercial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-accounts-api-openapi.yml
- filename: bbandt-corp-credit-transfers-account-list-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Credit Transfers Account List API
  slug: bbandt-corp-credit-transfers-account-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-credit-transfers-account-list-api-openapi.yml
- filename: bbandt-corp-credit-transfers-acknowledge-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Credit Transfers Acknowledge API
  slug: bbandt-corp-credit-transfers-acknowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-credit-transfers-acknowledge-api-openapi.yml
- filename: bbandt-corp-credit-transfers-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Credit Transfers API
  slug: bbandt-corp-credit-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-credit-transfers-api-openapi.yml
- filename: bbandt-corp-credit-transfers-approval-reject-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Credit Transfers Approval/Reject API
  slug: bbandt-corp-credit-transfers-approval-reject-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-credit-transfers-approval-reject-api-openapi.yml
- filename: bbandt-corp-event-notification-subscriptions-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Event Notification Subscriptions API
  slug: bbandt-corp-event-notification-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-event-notification-subscriptions-api-openapi.yml
- filename: bbandt-corp-event-notifications-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Event Notifications API
  slug: bbandt-corp-event-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-event-notifications-api-openapi.yml
- filename: bbandt-corp-location-information-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Location Information API
  slug: bbandt-corp-location-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-location-information-api-openapi.yml
- filename: bbandt-corp-money-movement-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Money Movement API
  slug: bbandt-corp-money-movement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-money-movement-api-openapi.yml
- filename: bbandt-corp-oauth-2-0-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) OAuth 2.0 API
  slug: bbandt-corp-oauth-2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-oauth-2-0-api-openapi.yml
- filename: bbandt-corp-personal-information-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Personal Information API
  slug: bbandt-corp-personal-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-personal-information-api-openapi.yml
- filename: bbandt-corp-recipients-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) Recipients API
  slug: bbandt-corp-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-recipients-api-openapi.yml
- filename: bbandt-corp-user-consent-api-openapi.yml
  format: yaml
  label: BB&T Corp (Truist) User Consent API
  slug: bbandt-corp-user-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-user-consent-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Bbandt Corp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BB&T Corp (Truist) secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BB&T Corp (Truist)
provider_slug: bbandt-corp
scheme_count: 2
schemes:
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/token
  name: OAuth
  sources:
  - openapi/bbandt-corp-commercial-account-balance-openapi.yml
  - openapi/bbandt-corp-commercial-account-transactions-openapi.yml
  - openapi/bbandt-corp-commercial-accounts-openapi.yml
  - openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml
  - openapi/bbandt-corp-retail-accounts-contact-openapi.yml
  - openapi/bbandt-corp-retail-accounts-openapi.yml
  - openapi/bbandt-corp-retail-accounts-transaction-openapi.yml
  - openapi/bbandt-corp-retail-auth-oauth-openapi.yml
  - openapi/bbandt-corp-retail-customers-openapi.yml
  - openapi/bbandt-corp-retail-payment-networks-openapi.yml
  type: oauth2
- description: This is the standard Basic Auth scheme encoded as `Base64(client_id:client_secret)`. Both Data Access Platforms and Direct Data Recipients MUST use the DAP/DDR client_id and client_secret returned from creating their Staging or Production application in Truist Developer Center. (You CANNOT use the Basic Auth credentials for a Data Recipient returned from dynamic client registration via `POST /regi
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/bbandt-corp-retail-auth-oauth-openapi.yml
  - openapi/bbandt-corp-retail-consents-openapi.yml
  - openapi/bbandt-corp-retail-event-notifications-openapi.yml
  - openapi/bbandt-corp-retail-event-subscriptions-openapi.yml
  - openapi/bbandt-corp-retail-locator-openapi.yml
  - openapi/bbandt-corp-retail-register-recipient-openapi.yml
  type: http
slug: bbandt-corp-authentication
source_filename: bbandt-corp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/bbandt-corp-commercial-account-balance-openapi.yml, openapi/bbandt-corp-commercial-account-transactions-openapi.yml,\n  openapi/bbandt-corp-commercial-accounts-openapi.yml, openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml,\n  openapi/bbandt-corp-retail-accounts-contact-openapi.yml, openapi/bbandt-corp-retail-accounts-openapi.yml, openapi/bbandt-corp-retail-accounts-transaction-openapi.yml,\n  openapi/bbandt-corp-retail-auth-oauth-openapi.yml, openapi/bbandt-corp-retail-consents-openapi.yml, openapi/bbandt-corp-retail-customers-openapi.yml,\n  openapi/bbandt-corp-retail-event-notifications-openapi.yml, openapi/bbandt-corp-retail-event-subscriptions-openapi.yml\n  ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/authorize\n\
  \    tokenUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/token\n    scopes: 1\n  description: The production authorization URL will be provided after the onboarding process is completed.\n  sources:\n  - openapi/bbandt-corp-commercial-account-balance-openapi.yml\n  - openapi/bbandt-corp-commercial-account-transactions-openapi.yml\n  - openapi/bbandt-corp-commercial-accounts-openapi.yml\n  - openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml\n  - openapi/bbandt-corp-retail-accounts-contact-openapi.yml\n  - openapi/bbandt-corp-retail-accounts-openapi.yml\n  - openapi/bbandt-corp-retail-accounts-transaction-openapi.yml\n  - openapi/bbandt-corp-retail-auth-oauth-openapi.yml\n  - openapi/bbandt-corp-retail-customers-openapi.yml\n  - openapi/bbandt-corp-retail-payment-networks-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: This is the standard Basic Auth scheme encoded as `Base64(client_id:client_secret)`. Both Data Access\n   \
  \ Platforms and Direct Data Recipients MUST use the DAP/DDR client_id and client_secret returned from creating their\n    Staging or Production application in Truist Developer Center. (You CANNOT use the Basic Auth credentials for a Data\n    Recipient returned from dynamic client registration via `POST /regi\n  sources:\n  - openapi/bbandt-corp-retail-auth-oauth-openapi.yml\n  - openapi/bbandt-corp-retail-consents-openapi.yml\n  - openapi/bbandt-corp-retail-event-notifications-openapi.yml\n  - openapi/bbandt-corp-retail-event-subscriptions-openapi.yml\n  - openapi/bbandt-corp-retail-locator-openapi.yml\n  - openapi/bbandt-corp-retail-register-recipient-openapi.yml\ndocs: https://developer.truist.com/api/retail-oauth-authentication/documentation\nnote: 'Truist publishes a dedicated OAuth 2.0 API contract (openapi/bbandt-corp-retail-auth-oauth-openapi.yml, \"Truist\n  Retail OAuth 2.0 API, v3\") alongside the resource APIs. Two schemes are in play: OAuth 2.0 authorization_code with\n  per-customer\
  \ consent on the data and payment APIs, and HTTP Basic (Base64(client_id:client_secret)) on the OAuth, consent,\n  event, dynamic-registration and locator APIs. The narrative auth pages on the developer portal render only behind sign-in,\n  so this profile stays spec-derived. Production authorization/token URLs are issued at onboarding; the specs carry the\n  sandbox hosts. Credential trap: the Basic Auth credentials returned by RFC 7591 dynamic client registration CANNOT\n  be used on the token endpoint — Truist requires the DAP/DDR client_id and client_secret from the Developer Center application.'\nmtls: false\nopenid_connect: true\nopenid_connect_note: The OAuth API declares the OIDC scopes profile, email, phone and address and returns an id_token,\n  but no /.well-known/openid-configuration is served (probed 2026-09-04).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/authentication/bbandt-corp-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Banking
- Financial Services
- Open Banking
- Truist
- BB&T
- Fortune 500
---
