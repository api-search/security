---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deutsche-bank-dbapi-addresses-v2.json
  format: json
  label: Deutsche Bank API Program
  slug: deutsche-bank
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-bank/refs/heads/main/openapi/deutsche-bank-dbapi-addresses-v2.json
- filename: deutsche-bank-merchant-solution-callback-v2.json
  format: json
  label: Deutsche Bank Merchant Solutions
  slug: merchant-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-bank/refs/heads/main/openapi/deutsche-bank-merchant-solution-callback-v2.json
auth_types: []
description: 'Deutsche Bank''s dbAPI programme is an OAuth 2.0 / OpenID Connect estate. Every dbAPI operation is protected by one of three named OAuth 2.0 security schemes declared in the specs, and the Merchant Solutions REST APIs use a bearer JWT minted by their own security API. There is no API-key path onto customer data: the portal API key is only used by the developer portal itself to read the public swagger catalogue.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Deutsche Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deutsche Bank declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Deutsche Bank
provider_slug: deutsche-bank
scheme_count: 4
schemes:
- applies_to:
  - dbapi-addresses-v2
  - dbapi-ageCertificate-v1
  - dbapi-cashAccounts-v2
  - dbapi-creditCards-v1
  - dbapi-creditCardTransactions-v1
  - dbapi-customerSolvency-v1
  - dbapi-investments-assets-v1
  - dbapi-investments-earningTransactions-v1
  - dbapi-investments-orders-v1
  - dbapi-investments-performances-v1
  - dbapi-investments-reports-v1
  - dbapi-investments-securityAccounts-v1
  - dbapi-investments-securityTransactions-v1
  - dbapi-partners-v2
  - dbapi-payments-sepaInstantCreditTransfer-v3
  - dbapi-sepaCreditTransfer-v3
  - dbapi-sepaDirectDebit-v1
  - dbapi-subscriptions-v1
  - dbapi-transactionAnalysis-v1
  - dbapi-transactionAuthorization-v1
  - dbapi-transactions-v2
  - dbapi-verifyCustomer-v1
  authorizationUrl: https://simulator-api.db.com/gw/oidc/oauth2/authorize
  description: End-user delegated access. Used by the customer-data APIs - accounts, transactions, credit cards, addresses, partners, investments, payments. PKCE (S256) is supported and documented as a separate guide; code_challenge_methods_supported is ["S256"].
  flow: authorizationCode
  name: api_auth_code
  tokenUrl: https://simulator-api.db.com/gw/oidc/oauth2/token
  type: oauth2
- applies_to:
  - dbapi-banking-cashAccountOpenings-v1
  - dbapi-investments-espSecuritiesAccounts-v1
  - dbapi-loanOffers-privatebanking-v1
  - dbapi-loanOffers-privatebanking-v2
  - dbapi-processingOrders-v1
  - dbapi-processingOrders-v2
  description: Machine-to-machine access for the onboarding, lending and processing surfaces where no end user is present in the request.
  flow: clientCredentials
  name: api_client_credential
  tokenUrl: https://simulator-api.db.com/gw/oidc/oauth2/token
  type: oauth2
- applies_to:
  - dbapi-cashAccounts-v2
  - dbapi-creditCards-v1
  - dbapi-creditCardTransactions-v1
  - dbapi-investments-assets-v1
  - dbapi-investments-earningTransactions-v1
  - dbapi-investments-performances-v1
  - dbapi-investments-reports-v1
  - dbapi-investments-securityAccounts-v1
  - dbapi-investments-securityTransactions-v1
  - dbapi-payments-sepaInstantCreditTransfer-v3
  - dbapi-sepaCreditTransfer-v3
  - dbapi-sepaDirectDebit-v1
  - dbapi-subscriptions-v1
  - dbapi-transactionAuthorization-v1
  - dbapi-transactions-v2
  description: db Smart Access - the corporate product where authorisation is bound to the onboarding contract rather than to a per-request customer consent. Release 2026.03 moved this product onto a technical OAuth2 client-credentials flow with annual recertification.
  flow: clientCredentials
  name: api_db_smart_access
  tokenUrl: https://simulator-api.db.com/gw/oidc/oauth2/token
  type: oauth2
- applies_to:
  - merchant-solution-services-v2
  - merchant-solution-services-v2.1
  - merchant-solution-security-v2
  - oneid-fakerock-v1
  bearerFormat: JWT
  description: Merchant Solutions REST APIs and the OneID contract. The Merchant-Server II Security API (POST /token) mints the JWT that the Services API then consumes.
  name: bearerAuth
  scheme: bearer
  type: http
slug: deutsche-bank-authentication
source_filename: deutsche-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Deutsche Bank\nproviderId: deutsche-bank\ngenerated: '2026-09-06'\nmethod: searched\nsource: https://developer.db.com/apidocumentation/oauthflows/oauthintroduction\nderived_from: openapi/ (36 first-party OpenAPI 3.0.x documents, components.securitySchemes)\ndocs: https://developer.db.com/apidocumentation/oauthflows/oauthintroduction\ndescription: >-\n  Deutsche Bank's dbAPI programme is an OAuth 2.0 / OpenID Connect estate. Every dbAPI\n  operation is protected by one of three named OAuth 2.0 security schemes declared in the\n  specs, and the Merchant Solutions REST APIs use a bearer JWT minted by their own security\n  API. There is no API-key path onto customer data: the portal API key is only used by the\n  developer portal itself to read the public swagger catalogue.\nidentity_providers:\n  - name: dbAPI OAuth / OIDC provider (simulation)\n    issuer: https://simulator-api.db.com/gw/oidc/\n\
  \    discovery: https://simulator-api.db.com/gw/oidc/.well-known/openid-configuration\n    file: well-known/deutsche-bank-simulator-openid-configuration.json\n    status: 200\n  - name: Deutsche Bank corporate CIAM (ForgeRock AM) - developer portal login\n    issuer: https://cidp-eu.db.com/am/oauth2/global\n    discovery: https://cidp-eu.db.com/am/oauth2/global/.well-known/openid-configuration\n    file: well-known/deutsche-bank-cidp-openid-configuration.json\n    status: 200\nproduction_hosts:\n  - tenant: Deutsche Bank\n    base: https://api.db.com\n  - tenant: norisbank\n    base: https://api.norisbank.de\n  - tenant: Postbank\n    base: https://api.postbank.de\nsandbox_host: https://simulator-api.db.com\nschemes:\n  - name: api_auth_code\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://simulator-api.db.com/gw/oidc/oauth2/authorize\n    tokenUrl: https://simulator-api.db.com/gw/oidc/oauth2/token\n    description: >-\n      End-user delegated access. Used\
  \ by the customer-data APIs - accounts, transactions,\n      credit cards, addresses, partners, investments, payments. PKCE (S256) is supported and\n      documented as a separate guide; code_challenge_methods_supported is [\"S256\"].\n    applies_to:\n      - dbapi-addresses-v2\n      - dbapi-ageCertificate-v1\n      - dbapi-cashAccounts-v2\n      - dbapi-creditCards-v1\n      - dbapi-creditCardTransactions-v1\n      - dbapi-customerSolvency-v1\n      - dbapi-investments-assets-v1\n      - dbapi-investments-earningTransactions-v1\n      - dbapi-investments-orders-v1\n      - dbapi-investments-performances-v1\n      - dbapi-investments-reports-v1\n      - dbapi-investments-securityAccounts-v1\n      - dbapi-investments-securityTransactions-v1\n      - dbapi-partners-v2\n      - dbapi-payments-sepaInstantCreditTransfer-v3\n      - dbapi-sepaCreditTransfer-v3\n      - dbapi-sepaDirectDebit-v1\n      - dbapi-subscriptions-v1\n      - dbapi-transactionAnalysis-v1\n      - dbapi-transactionAuthorization-v1\n\
  \      - dbapi-transactions-v2\n      - dbapi-verifyCustomer-v1\n  - name: api_client_credential\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://simulator-api.db.com/gw/oidc/oauth2/token\n    description: >-\n      Machine-to-machine access for the onboarding, lending and processing surfaces where no\n      end user is present in the request.\n    applies_to:\n      - dbapi-banking-cashAccountOpenings-v1\n      - dbapi-investments-espSecuritiesAccounts-v1\n      - dbapi-loanOffers-privatebanking-v1\n      - dbapi-loanOffers-privatebanking-v2\n      - dbapi-processingOrders-v1\n      - dbapi-processingOrders-v2\n  - name: api_db_smart_access\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://simulator-api.db.com/gw/oidc/oauth2/token\n    description: >-\n      db Smart Access - the corporate product where authorisation is bound to the onboarding\n      contract rather than to a per-request customer consent. Release 2026.03 moved this\n      product\
  \ onto a technical OAuth2 client-credentials flow with annual recertification.\n    applies_to:\n      - dbapi-cashAccounts-v2\n      - dbapi-creditCards-v1\n      - dbapi-creditCardTransactions-v1\n      - dbapi-investments-assets-v1\n      - dbapi-investments-earningTransactions-v1\n      - dbapi-investments-performances-v1\n      - dbapi-investments-reports-v1\n      - dbapi-investments-securityAccounts-v1\n      - dbapi-investments-securityTransactions-v1\n      - dbapi-payments-sepaInstantCreditTransfer-v3\n      - dbapi-sepaCreditTransfer-v3\n      - dbapi-sepaDirectDebit-v1\n      - dbapi-subscriptions-v1\n      - dbapi-transactionAuthorization-v1\n      - dbapi-transactions-v2\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Merchant Solutions REST APIs and the OneID contract. The Merchant-Server II Security API\n      (POST /token) mints the JWT that the Services API then consumes.\n    applies_to:\n      - merchant-solution-services-v2\n\
  \      - merchant-solution-services-v2.1\n      - merchant-solution-security-v2\n      - oneid-fakerock-v1\ngrant_types:\n  - authorization_code\n  - authorization_code + PKCE (S256)\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\nclient_authentication:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\n  - self_signed_tls_client_auth\nmutual_tls:\n  supported: true\n  note: >-\n    The dbAPI OIDC discovery document advertises tls_client_auth and\n    self_signed_tls_client_auth, and tls_client_certificate_bound_access_tokens is true. The\n    portal documents this as \"Certificate based Authentication\".\n  docs: https://developer.db.com/apidocumentation/oauthflows/certificates\nstep_up:\n  present: true\n  mechanism: >-\n    Strong customer authentication (PSD2 SCA) is a first-class API surface. The Transaction\n    Authorization\
  \ API issues and verifies challenges (PushTAN and other methods), and payment\n    and investment write operations carry an OTP request header that carries the second\n    factor.\n  api: dbapi-transactionAuthorization-v1\n  headers:\n    - OTP\n    - otp\nscopes: scopes/deutsche-bank-scopes.yml\ncommon_headers:\n  - name: Correlation-Id\n    required_on: every operation in the dbAPI estate\n    description: Caller-supplied correlation identifier for request tracing.\n  - name: idempotency-id\n    format: uuid\n    description: Replay-protection key on the write surfaces that support it. See conventions/.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutsche-bank/refs/heads/main/authentication/deutsche-bank-authentication.yml
summary_line: 4 schemes
tags:
- Banking
- Financial
- Wealth Management
- Open Banking
- PSD2
- Payments
- SEPA
- Investments
- Credit Cards
- Merchant Solutions
- Germany
- Financial Services
---
