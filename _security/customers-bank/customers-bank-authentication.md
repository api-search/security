---
api_key_in: []
api_specs:
- filename: customers-bank-accounts-openapi.json
  format: json
  label: Customers Bank Accounts API
  slug: customers-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-accounts-openapi.json
- filename: customers-bank-ach-openapi.json
  format: json
  label: Customers Bank ACH API
  slug: customers-bank-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-ach-openapi.json
- filename: customers-bank-consumerlending-openapi.json
  format: json
  label: Customers Bank Consumer Lending API
  slug: customers-bank-consumer-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-consumerlending-openapi.json
- filename: customers-bank-instantpayments-openapi.json
  format: json
  label: Customers Bank Instant Payments API
  slug: customers-bank-instant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-instantpayments-openapi.json
- filename: customers-bank-itoperations-openapi.json
  format: json
  label: Customers Bank IT Operations API
  slug: customers-bank-it-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-itoperations-openapi.json
- filename: customers-bank-partners-openapi.json
  format: json
  label: Customers Bank Partners API
  slug: customers-bank-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-partners-openapi.json
- filename: customers-bank-security-openapi.json
  format: json
  label: Customers Bank Security API
  slug: customers-bank-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-security-openapi.json
- filename: customers-bank-transfers-openapi.json
  format: json
  label: Customers Bank Transfers API
  slug: customers-bank-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-transfers-openapi.json
- filename: customers-bank-webhooks-openapi.json
  format: json
  label: Customers Bank Webhooks API
  slug: customers-bank-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-webhooks-openapi.json
- filename: customers-bank-wires-openapi.json
  format: json
  label: Customers Bank Wires API
  slug: customers-bank-wires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-wires-openapi.json
auth_types:
- oauth2
- http-bearer
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Customers Bank Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Customers Bank secures its APIs with oauth2, http-bearer, and hmac across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Customers Bank
provider_slug: customers-bank
scheme_count: 3
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  note: client_Id is a UUID; client_Secret is up to 40 chars (shown once at creation). Cache the token for expires_in seconds. Credentials are provisioned via the Partners API (client-credentials / M2M application registration).
  parameters:
  - client_Id
  - client_Secret
  - grant_type
  request_content_type: application/x-www-form-urlencoded
  scopes: none-documented
  token_lifetime_seconds: 3600
  token_type: Bearer
  token_url: https://cubi-sandbox-api.customersbank.com/security/v1/oauth2/token
  type: oauth2
- applies_to: All resource APIs (accounts, ach, wires, instant payments, transfers, consumer lending, partners, webhooks, it-operations)
  header: 'Authorization: Bearer {access_token}'
  name: BearerAuth
  scheme: bearer
  type: http
- algorithm: HMAC-SHA256
  applies_to: Webhook callback delivery to the subscriber callbackUrl
  direction: inbound-callback
  docs: https://cubiapi.readme.io/docs/hmac-signature-validation
  headers:
  - Authorization
  - Authorization-Timestamp
  - X-Event-Type
  name: WebhookHMAC
  secret: secretText (Base64-encoded) supplied at webhook subscription time
  signature_format: 'Authorization: HMAC-SHA256 Signature={base64}'
  type: hmac
slug: customers-bank-authentication
source_filename: customers-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://cubiapi.readme.io/docs/authenticate-1\ndocs: https://cubiapi.readme.io/docs/authenticate-1\nnote: >-\n  The OpenAPI documents do not declare securitySchemes in-spec; the auth model is documented\n  in the ReadMe developer portal. Access is machine-to-machine OAuth2 client-credentials;\n  webhook callbacks are authenticated separately with HMAC-SHA256 signatures.\nsummary:\n  types: [oauth2, http-bearer, hmac]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://cubi-sandbox-api.customersbank.com/security/v1/oauth2/token\n    grant_type: client_credentials\n    request_content_type: application/x-www-form-urlencoded\n    parameters: [client_Id, client_Secret, grant_type]\n    token_type: Bearer\n    token_lifetime_seconds: 3600\n    scopes: none-documented\n    note: >-\n      client_Id is a UUID; client_Secret\
  \ is up to 40 chars (shown once at creation).\n      Cache the token for expires_in seconds. Credentials are provisioned via the Partners API\n      (client-credentials / M2M application registration).\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    applies_to: All resource APIs (accounts, ach, wires, instant payments, transfers, consumer lending, partners, webhooks, it-operations)\n    header: 'Authorization: Bearer {access_token}'\n  - name: WebhookHMAC\n    type: hmac\n    algorithm: HMAC-SHA256\n    direction: inbound-callback\n    applies_to: Webhook callback delivery to the subscriber callbackUrl\n    headers: [Authorization, Authorization-Timestamp, X-Event-Type]\n    signature_format: 'Authorization: HMAC-SHA256 Signature={base64}'\n    secret: secretText (Base64-encoded) supplied at webhook subscription time\n    docs: https://cubiapi.readme.io/docs/hmac-signature-validation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/authentication/customers-bank-authentication.yml
summary_line: oauth2/http-bearer/hmac · 3 schemes
tags:
- Financial Services
- Banking
- United States
- Banking-as-a-Service
- Embedded Finance
- Payments
- Commercial Banking
---
