---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: citi-authentication-api-1-openapi.yaml
  format: yaml
  label: Citi API Authentication Services
  slug: citi-api-authentication-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-authentication-api-1-openapi.yaml
- filename: citi-blocksandfilters-openapi.yaml
  format: yaml
  label: Citi Account Reporting APIs
  slug: citi-account-reporting-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-blocksandfilters-openapi.yaml
- filename: citi-digitalpaymentscollectionsv12-openapi.yaml
  format: yaml
  label: Citi Outgoing Payments APIs
  slug: citi-outgoing-payments-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-digitalpaymentscollectionsv12-openapi.yaml
- filename: citi-brazillocalmandate-openapi.yaml
  format: yaml
  label: Citi Payment Acceptance APIs
  slug: citi-payment-acceptance-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-brazillocalmandate-openapi.yaml
- filename: citi-marqueta-openapi.yaml
  format: yaml
  label: Citi Commercial Cards and Virtual Card Accounts APIs
  slug: citi-commercial-cards-and-virtual-card-accounts-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-marqueta-openapi.yaml
- filename: citi-fx-authentication-api-openapi.yaml
  format: yaml
  label: CitiFX Gateway and Instant FX APIs
  slug: citifx-gateway-and-instant-fx-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-fx-authentication-api-openapi.yaml
- filename: citi-custody-billing-openapi.yaml
  format: yaml
  label: Citi Custody and Securities Services APIs
  slug: citi-custody-and-securities-services-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-custody-billing-openapi.yaml
- filename: citi-transfer-agency-accounts-openapi.yaml
  format: yaml
  label: Citi Funds Transfer Agency APIs
  slug: citi-funds-transfer-agency-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-transfer-agency-accounts-openapi.yaml
- filename: citi-ukraine-bank-data-sharing-api-openapi.yaml
  format: yaml
  label: Citi Open Banking APIs
  slug: citi-open-banking-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-ukraine-bank-data-sharing-api-openapi.yaml
- filename: citi-finance-undertaking-api-openapi.yaml
  format: yaml
  label: CitiConnect Trade Services APIs
  slug: citiconnect-trade-services-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-finance-undertaking-api-openapi.yaml
- filename: citi-marketplace-management-openapi.yaml
  format: yaml
  label: Citi Gateway Services API
  slug: citi-gateway-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-marketplace-management-openapi.yaml
- filename: citi-self-service-api-openapi.yaml
  format: yaml
  label: Citi Additional Payment Services APIs
  slug: citi-additional-payment-services-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-self-service-api-openapi.yaml
auth_types:
- apiKey
- http
- oauth2
- unknown
description: ''
kind: authentication
layout: security
mechanism_count: 9
method: derived
name: Citi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Citi secures its APIs with apiKey, http, oauth2, and unknown across 10 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Citi
provider_slug: citi
scheme_count: 10
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
  name: clientCredentials
  sources:
  - openapi/citi-account-balance-inquiry-api-openapi.yaml
  - openapi/citi-account-notifications-api-openapi.yaml
  - openapi/citi-accounts-openapi.yaml
  - openapi/citi-accountsv5-openapi.yaml
  - openapi/citi-addonservice-openapi.yaml
  - openapi/citi-balances-api-openapi.yaml
  - openapi/citi-beneficiary-search-openapi.yaml
  - openapi/citi-blocksandfilters-openapi.yaml
  - openapi/citi-bulk-payments-openapi.yaml
  - openapi/citi-card-disputes-openapi.yaml
  - openapi/citi-cash-balances-openapi.yaml
  - openapi/citi-cash-transactions-openapi.yaml
  - openapi/citi-clearing-exception-report-openapi.yaml
  - openapi/citi-custody-billing-openapi.yaml
  - openapi/citi-custody-fx-transactions-openapi.yaml
  - openapi/citi-custody-penalties-openapi.yaml
  - openapi/citi-direct-debit-api-openapi.yaml
  - openapi/citi-due-date-openapi.yaml
  - openapi/citi-e-mandate-api-v1-openapi.yaml
  - openapi/citi-e-mandate-api-v2-openapi.yaml
  - openapi/citi-finance-undertaking-api-openapi.yaml
  - openapi/citi-fx-benchmark-async-api-openapi.yaml
  - openapi/citi-fx-benchmark-sync-api-openapi.yaml
  - openapi/citi-fx-cancel-async-api-openapi.yaml
  - openapi/citi-fx-cancel-sync-api-openapi.yaml
  - openapi/citi-fx-ecommerce-api-openapi.yaml
  - openapi/citi-fx-gateway-reporting-async-api-openapi.yaml
  - openapi/citi-fx-gateway-reporting-sync-api-openapi.yaml
  - openapi/citi-fx-market-async-api-openapi.yaml
  - openapi/citi-fx-market-sync-api-openapi.yaml
  - openapi/citi-fx-orders-async-api-openapi.yaml
  - openapi/citi-fx-orders-sync-api-openapi.yaml
  - openapi/citi-fx-quote-async-api-openapi.yaml
  - openapi/citi-fx-quote-sync-api-openapi.yaml
  - openapi/citi-fx-reporting-async-api-openapi.yaml
  - openapi/citi-fx-reporting-sync-api-openapi.yaml
  - openapi/citi-grace-iva-openapi.yaml
  - openapi/citi-id-provisioning-openapi.yaml
  - openapi/citi-immediate-openapi.yaml
  - openapi/citi-marketplace-management-openapi.yaml
  - openapi/citi-marqueta-openapi.yaml
  - openapi/citi-mobile-wallets-openapi.yaml
  - openapi/citi-mobilecardonboarding-openapi.yaml
  - openapi/citi-mobilevirtuallifecycle-openapi.yaml
  - openapi/citi-online-payment-acceptance-api-openapi.yaml
  - openapi/citi-order-approval-openapi.yaml
  - openapi/citi-payerid-api-openapi.yaml
  - openapi/citi-payment-reconfirmation-openapi.yaml
  - openapi/citi-payment-refund-openapi.yaml
  - openapi/citi-payment-status-openapi.yaml
  - openapi/citi-paymentcancellation-json-openapi.yaml
  - openapi/citi-paymentcancellation-xml-openapi.yaml
  - openapi/citi-paymentenhancedinquiry-json-openapi.yaml
  - openapi/citi-paymentenhancedinquiry-xml-openapi.yaml
  - openapi/citi-paymentinitiation-pacs008-openapi.yaml
  - openapi/citi-paymentinitiation-pacs009-openapi.yaml
  - openapi/citi-paymentinitiation-pain102-openapi.yaml
  - openapi/citi-paymentinitiation-pain103-openapi.yaml
  - openapi/citi-payto-openapi.yaml
  - openapi/citi-portfolio-listing-openapi.yaml
  - openapi/citi-purchase-openapi.yaml
  - openapi/citi-reporting-get-2-openapi.yaml
  - openapi/citi-request-to-pay-openapi.yaml
  - openapi/citi-safekeeping-accounts-openapi.yaml
  - openapi/citi-safekeeping-positions-openapi.yaml
  - openapi/citi-securitytransactionsaccounts-openapi.yaml
  - openapi/citi-self-service-api-openapi.yaml
  - openapi/citi-statement-transactions-openapi.yaml
  - openapi/citi-statements-api-openapi.yaml
  - openapi/citi-submit-action-openapi.yaml
  - openapi/citi-tax-reclaims-openapi.yaml
  - openapi/citi-trade-api-openapi.yaml
  - openapi/citi-transfer-agency-accounts-openapi.yaml
  - openapi/citi-transfer-agency-holding-openapi.yaml
  - openapi/citi-transfer-agency-investors-openapi.yaml
  - openapi/citi-transfer-agency-transactions-openapi.yaml
  - openapi/citi-ukraine-bank-data-sharing-api-openapi.yaml
  - openapi/citi-ukraine-payment-service-initiation-api-openapi.yaml
  - openapi/citi-vamanagement-openapi.yaml
  - openapi/citi-vca-api-openapi.yaml
  - openapi/citi-vcaeventssubscriptions-openapi.yaml
  - openapi/citi-vcagetnotifications-openapi.yaml
  - openapi/citi-virtual-cards-lifecycle-v1-openapi.yaml
  - openapi/citi-virtual-cards-lifecycle-v4-openapi.yaml
  - openapi/citi-virtual-cards-notifications-openapi.yaml
  - openapi/citi-virtual-cards-pi-openapi.yaml
  - openapi/citi-virtual-cards-pi-v2-openapi.yaml
  - openapi/citi-virtual-cards-reporting-openapi.yaml
  - openapi/citi-virtual-cards-reporting-v1-openapi.yaml
  - openapi/citi-worldlink-ir-api-openapi.yaml
  - openapi/citi-worldlink-v1-api-openapi.yaml
  - openapi/citi-worldlink-v2-api-openapi.yaml
  - openapi/citi-worldlink-v3-api-openapi.yaml
  - openapi/citi-worldlink-v5-api-openapi.yaml
  type: oauth2
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    scopes: 2
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  sources:
  - openapi/citi-add-on-service-openapi.yaml
  - openapi/citi-brazillocalmandate-openapi.yaml
  - openapi/citi-contractstatusinquiry-openapi.yaml
  - openapi/citi-digitalpaymentscollectionsv12-openapi.yaml
  - openapi/citi-entityid-openapi.yaml
  - openapi/citi-express-payments-api-openapi.yaml
  - openapi/citi-express-payments-webhooks-openapi.yaml
  - openapi/citi-idd-openapi.yaml
  - openapi/citi-proof-of-payment-openapi.yaml
  - openapi/citi-statementsv2-api-openapi.yaml
  - openapi/citi-static-openapi.yaml
  - openapi/citi-virtual-cards-pi-webhooks-openapi.yaml
  type: oauth2
- description: Username is the application's client_id and password is the client_secret.
  name: Basic Authentication
  scheme: basic
  sources:
  - openapi/citi-authentication-api-1-openapi.yaml
  - openapi/citi-authentication-api-2-openapi.yaml
  - openapi/citi-authentication-api-3-openapi.yaml
  - openapi/citi-authentication-api-4-openapi.yaml
  - openapi/citi-fx-authentication-api-openapi.yaml
  - openapi/citi-ukraine-open-banking-authentication-api-openapi.yaml
  - openapi/citi-virtual-cards-pi-webhooks-openapi.yaml
  type: http
- in: header
  name: clientIdHeader
  parameter: X-IBM-Client-Id
  sources:
  - openapi/citi-authentication-api-1-openapi.yaml
  - openapi/citi-authentication-api-2-openapi.yaml
  - openapi/citi-authentication-api-3-openapi.yaml
  - openapi/citi-authentication-api-4-openapi.yaml
  - openapi/citi-ukraine-open-banking-authentication-api-openapi.yaml
  type: apiKey
- in: header
  name: clientSecretHeader
  parameter: X-IBM-Client-Secret
  sources:
  - openapi/citi-authentication-api-1-openapi.yaml
  - openapi/citi-authentication-api-2-openapi.yaml
  - openapi/citi-authentication-api-3-openapi.yaml
  - openapi/citi-authentication-api-4-openapi.yaml
  - openapi/citi-ukraine-open-banking-authentication-api-openapi.yaml
  type: apiKey
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  name: clientCredentials
  sources:
  - openapi/citi-digitalpaymentscollectionsv12-openapi.yaml
  type: unknown
- bearerFormat: opaque OAuth 2.0
  description: The access token obtained as a result of OAuth 2.0 flows.
  name: oauthBearerToken
  scheme: bearer
  sources:
  - openapi/citi-finance-undertaking-api-openapi.yaml
  type: http
- in: query
  name: client_id
  parameter: client_id
  sources:
  - openapi/citi-fx-benchmark-async-api-openapi.yaml
  - openapi/citi-fx-benchmark-sync-api-openapi.yaml
  - openapi/citi-fx-cancel-async-api-openapi.yaml
  - openapi/citi-fx-cancel-sync-api-openapi.yaml
  - openapi/citi-fx-ecommerce-api-openapi.yaml
  - openapi/citi-fx-gateway-reporting-async-api-openapi.yaml
  - openapi/citi-fx-gateway-reporting-sync-api-openapi.yaml
  - openapi/citi-fx-market-async-api-openapi.yaml
  - openapi/citi-fx-market-sync-api-openapi.yaml
  - openapi/citi-payment-reconfirmation-openapi.yaml
  - openapi/citi-payment-refund-openapi.yaml
  - openapi/citi-payment-status-openapi.yaml
  type: apiKey
- description: Mutual TLS (mTLS) authentication. Both root and intermediary certificates must be exchanged with the API provider as part of the formal onboarding process before any API calls can be made.
  name: mutualTLS
  scheme: mutual-tls
  sources:
  - openapi/citi-vca-dual-auth-authorization-openapi.yaml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/citi-virtual-cards-pi-webhooks-openapi.yaml
  type: apiKey
slug: citi-authentication
source_filename: citi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/citi-account-balance-inquiry-api-openapi.yaml, openapi/citi-account-notifications-api-openapi.yaml,\n  openapi/citi-accounts-openapi.yaml, openapi/citi-accountsv5-openapi.yaml, openapi/citi-add-on-service-openapi.yaml,\n  openapi/citi-addonservice-openapi.yaml, openapi/citi-authentication-api-1-openapi.yaml, openapi/citi-authentication-api-2-openapi.yaml,\n  openapi/citi-authentication-api-3-openapi.yaml, openapi/citi-authentication-api-4-openapi.yaml,\n  openapi/citi-balances-api-openapi.yaml, openapi/citi-beneficiary-search-openapi.yaml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - unknown\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: clientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/citi-account-balance-inquiry-api-openapi.yaml\n\
  \  - openapi/citi-account-notifications-api-openapi.yaml\n  - openapi/citi-accounts-openapi.yaml\n  - openapi/citi-accountsv5-openapi.yaml\n  - openapi/citi-addonservice-openapi.yaml\n  - openapi/citi-balances-api-openapi.yaml\n  - openapi/citi-beneficiary-search-openapi.yaml\n  - openapi/citi-blocksandfilters-openapi.yaml\n  - openapi/citi-bulk-payments-openapi.yaml\n  - openapi/citi-card-disputes-openapi.yaml\n  - openapi/citi-cash-balances-openapi.yaml\n  - openapi/citi-cash-transactions-openapi.yaml\n  - openapi/citi-clearing-exception-report-openapi.yaml\n  - openapi/citi-custody-billing-openapi.yaml\n  - openapi/citi-custody-fx-transactions-openapi.yaml\n  - openapi/citi-custody-penalties-openapi.yaml\n  - openapi/citi-direct-debit-api-openapi.yaml\n  - openapi/citi-due-date-openapi.yaml\n  - openapi/citi-e-mandate-api-v1-openapi.yaml\n  - openapi/citi-e-mandate-api-v2-openapi.yaml\n  - openapi/citi-finance-undertaking-api-openapi.yaml\n  - openapi/citi-fx-benchmark-async-api-openapi.yaml\n\
  \  - openapi/citi-fx-benchmark-sync-api-openapi.yaml\n  - openapi/citi-fx-cancel-async-api-openapi.yaml\n  - openapi/citi-fx-cancel-sync-api-openapi.yaml\n  - openapi/citi-fx-ecommerce-api-openapi.yaml\n  - openapi/citi-fx-gateway-reporting-async-api-openapi.yaml\n  - openapi/citi-fx-gateway-reporting-sync-api-openapi.yaml\n  - openapi/citi-fx-market-async-api-openapi.yaml\n  - openapi/citi-fx-market-sync-api-openapi.yaml\n  - openapi/citi-fx-orders-async-api-openapi.yaml\n  - openapi/citi-fx-orders-sync-api-openapi.yaml\n  - openapi/citi-fx-quote-async-api-openapi.yaml\n  - openapi/citi-fx-quote-sync-api-openapi.yaml\n  - openapi/citi-fx-reporting-async-api-openapi.yaml\n  - openapi/citi-fx-reporting-sync-api-openapi.yaml\n  - openapi/citi-grace-iva-openapi.yaml\n  - openapi/citi-id-provisioning-openapi.yaml\n  - openapi/citi-immediate-openapi.yaml\n  - openapi/citi-marketplace-management-openapi.yaml\n  - openapi/citi-marqueta-openapi.yaml\n  - openapi/citi-mobile-wallets-openapi.yaml\n\
  \  - openapi/citi-mobilecardonboarding-openapi.yaml\n  - openapi/citi-mobilevirtuallifecycle-openapi.yaml\n  - openapi/citi-online-payment-acceptance-api-openapi.yaml\n  - openapi/citi-order-approval-openapi.yaml\n  - openapi/citi-payerid-api-openapi.yaml\n  - openapi/citi-payment-reconfirmation-openapi.yaml\n  - openapi/citi-payment-refund-openapi.yaml\n  - openapi/citi-payment-status-openapi.yaml\n  - openapi/citi-paymentcancellation-json-openapi.yaml\n  - openapi/citi-paymentcancellation-xml-openapi.yaml\n  - openapi/citi-paymentenhancedinquiry-json-openapi.yaml\n  - openapi/citi-paymentenhancedinquiry-xml-openapi.yaml\n  - openapi/citi-paymentinitiation-pacs008-openapi.yaml\n  - openapi/citi-paymentinitiation-pacs009-openapi.yaml\n  - openapi/citi-paymentinitiation-pain102-openapi.yaml\n  - openapi/citi-paymentinitiation-pain103-openapi.yaml\n  - openapi/citi-payto-openapi.yaml\n  - openapi/citi-portfolio-listing-openapi.yaml\n  - openapi/citi-purchase-openapi.yaml\n  - openapi/citi-reporting-get-2-openapi.yaml\n\
  \  - openapi/citi-request-to-pay-openapi.yaml\n  - openapi/citi-safekeeping-accounts-openapi.yaml\n  - openapi/citi-safekeeping-positions-openapi.yaml\n  - openapi/citi-securitytransactionsaccounts-openapi.yaml\n  - openapi/citi-self-service-api-openapi.yaml\n  - openapi/citi-statement-transactions-openapi.yaml\n  - openapi/citi-statements-api-openapi.yaml\n  - openapi/citi-submit-action-openapi.yaml\n  - openapi/citi-tax-reclaims-openapi.yaml\n  - openapi/citi-trade-api-openapi.yaml\n  - openapi/citi-transfer-agency-accounts-openapi.yaml\n  - openapi/citi-transfer-agency-holding-openapi.yaml\n  - openapi/citi-transfer-agency-investors-openapi.yaml\n  - openapi/citi-transfer-agency-transactions-openapi.yaml\n  - openapi/citi-ukraine-bank-data-sharing-api-openapi.yaml\n  - openapi/citi-ukraine-payment-service-initiation-api-openapi.yaml\n  - openapi/citi-vamanagement-openapi.yaml\n  - openapi/citi-vca-api-openapi.yaml\n  - openapi/citi-vcaeventssubscriptions-openapi.yaml\n  - openapi/citi-vcagetnotifications-openapi.yaml\n\
  \  - openapi/citi-virtual-cards-lifecycle-v1-openapi.yaml\n  - openapi/citi-virtual-cards-lifecycle-v4-openapi.yaml\n  - openapi/citi-virtual-cards-notifications-openapi.yaml\n  - openapi/citi-virtual-cards-pi-openapi.yaml\n  - openapi/citi-virtual-cards-pi-v2-openapi.yaml\n  - openapi/citi-virtual-cards-reporting-openapi.yaml\n  - openapi/citi-virtual-cards-reporting-v1-openapi.yaml\n  - openapi/citi-worldlink-ir-api-openapi.yaml\n  - openapi/citi-worldlink-v1-api-openapi.yaml\n  - openapi/citi-worldlink-v2-api-openapi.yaml\n  - openapi/citi-worldlink-v3-api-openapi.yaml\n  - openapi/citi-worldlink-v5-api-openapi.yaml\n- name: clientCredentials\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authenticationservices/v3/oauth/token\n    tokenUrl: /authenticationservices/v3/oauth/token\n    scopes: 2\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes\
  \ the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n  sources:\n  - openapi/citi-add-on-service-openapi.yaml\n  - openapi/citi-brazillocalmandate-openapi.yaml\n  - openapi/citi-contractstatusinquiry-openapi.yaml\n  - openapi/citi-digitalpaymentscollectionsv12-openapi.yaml\n  - openapi/citi-entityid-openapi.yaml\n  - openapi/citi-express-payments-api-openapi.yaml\n  - openapi/citi-express-payments-webhooks-openapi.yaml\n  - openapi/citi-idd-openapi.yaml\n  - openapi/citi-proof-of-payment-openapi.yaml\n  - openapi/citi-statementsv2-api-openapi.yaml\n  - openapi/citi-static-openapi.yaml\n  - openapi/citi-virtual-cards-pi-webhooks-openapi.yaml\n- name: Basic Authentication\n  type: http\n  scheme: basic\n  description: Username is the application's client_id and password is the client_secret.\n  sources:\n  - openapi/citi-authentication-api-1-openapi.yaml\n\
  \  - openapi/citi-authentication-api-2-openapi.yaml\n  - openapi/citi-authentication-api-3-openapi.yaml\n  - openapi/citi-authentication-api-4-openapi.yaml\n  - openapi/citi-fx-authentication-api-openapi.yaml\n  - openapi/citi-ukraine-open-banking-authentication-api-openapi.yaml\n  - openapi/citi-virtual-cards-pi-webhooks-openapi.yaml\n- name: clientIdHeader\n  type: apiKey\n  in: header\n  parameter: X-IBM-Client-Id\n  sources:\n  - openapi/citi-authentication-api-1-openapi.yaml\n  - openapi/citi-authentication-api-2-openapi.yaml\n  - openapi/citi-authentication-api-3-openapi.yaml\n  - openapi/citi-authentication-api-4-openapi.yaml\n  - openapi/citi-ukraine-open-banking-authentication-api-openapi.yaml\n- name: clientSecretHeader\n  type: apiKey\n  in: header\n  parameter: X-IBM-Client-Secret\n  sources:\n  - openapi/citi-authentication-api-1-openapi.yaml\n  - openapi/citi-authentication-api-2-openapi.yaml\n  - openapi/citi-authentication-api-3-openapi.yaml\n  - openapi/citi-authentication-api-4-openapi.yaml\n\
  \  - openapi/citi-ukraine-open-banking-authentication-api-openapi.yaml\n- name: clientCredentials\n  type: unknown\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n  sources:\n  - openapi/citi-digitalpaymentscollectionsv12-openapi.yaml\n- name: oauthBearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: opaque OAuth 2.0\n  description: The access token obtained as a result of OAuth 2.0 flows.\n  sources:\n  - openapi/citi-finance-undertaking-api-openapi.yaml\n- name: client_id\n  type: apiKey\n  in: query\n  parameter: client_id\n  sources:\n  - openapi/citi-fx-benchmark-async-api-openapi.yaml\n  - openapi/citi-fx-benchmark-sync-api-openapi.yaml\n\
  \  - openapi/citi-fx-cancel-async-api-openapi.yaml\n  - openapi/citi-fx-cancel-sync-api-openapi.yaml\n  - openapi/citi-fx-ecommerce-api-openapi.yaml\n  - openapi/citi-fx-gateway-reporting-async-api-openapi.yaml\n  - openapi/citi-fx-gateway-reporting-sync-api-openapi.yaml\n  - openapi/citi-fx-market-async-api-openapi.yaml\n  - openapi/citi-fx-market-sync-api-openapi.yaml\n  - openapi/citi-payment-reconfirmation-openapi.yaml\n  - openapi/citi-payment-refund-openapi.yaml\n  - openapi/citi-payment-status-openapi.yaml\n- name: mutualTLS\n  type: http\n  scheme: mutual-tls\n  description: Mutual TLS (mTLS) authentication. Both root and intermediary certificates must\n    be exchanged with the API provider as part of the formal onboarding process before any API\n    calls can be made.\n  sources:\n  - openapi/citi-vca-dual-auth-authorization-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/citi-virtual-cards-pi-webhooks-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/authentication/citi-authentication.yml
summary_line: apiKey/http/oauth2/unknown · 10 schemes
tags:
- Banking
- Financial-Services
- Open Banking
- Payments
- Treasury
- ISO 20022
- Commercial Cards
- Foreign Exchange
- Custody
- Trade Finance
- Corporate Banking
- API Gateway
---
