---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pliant-account-entries-api-openapi.yml
  format: yaml
  label: Pliant Account Entries API
  slug: pliant-account-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-account-entries-api-openapi.yml
- filename: pliant-accounting-projects-api-openapi.yml
  format: yaml
  label: Pliant Accounting Projects API
  slug: pliant-accounting-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-accounting-projects-api-openapi.yml
- filename: pliant-accounting-teams-api-openapi.yml
  format: yaml
  label: Pliant Accounting Teams API
  slug: pliant-accounting-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-accounting-teams-api-openapi.yml
- filename: pliant-accounting-transactions-api-openapi.yml
  format: yaml
  label: Pliant Accounting Transactions API
  slug: pliant-accounting-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-accounting-transactions-api-openapi.yml
- filename: pliant-callbacks-api-openapi.yml
  format: yaml
  label: Pliant Callbacks API
  slug: pliant-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-callbacks-api-openapi.yml
- filename: pliant-card-accounts-api-openapi.yml
  format: yaml
  label: Pliant Card Accounts API
  slug: pliant-card-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-card-accounts-api-openapi.yml
- filename: pliant-card-controls-api-openapi.yml
  format: yaml
  label: Pliant Card Controls API
  slug: pliant-card-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-card-controls-api-openapi.yml
- filename: pliant-card-copilots-api-openapi.yml
  format: yaml
  label: Pliant Card Copilots API
  slug: pliant-card-copilots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-card-copilots-api-openapi.yml
- filename: pliant-card-sensitive-data-api-openapi.yml
  format: yaml
  label: Pliant Card Sensitive Data API
  slug: pliant-card-sensitive-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-card-sensitive-data-api-openapi.yml
- filename: pliant-cardholders-api-openapi.yml
  format: yaml
  label: Pliant Cardholders API
  slug: pliant-cardholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-cardholders-api-openapi.yml
- filename: pliant-cards-api-openapi.yml
  format: yaml
  label: Pliant Cards API
  slug: pliant-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-cards-api-openapi.yml
- filename: pliant-custom-fields-api-openapi.yml
  format: yaml
  label: Pliant Custom Fields API
  slug: pliant-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-custom-fields-api-openapi.yml
- filename: pliant-organizations-api-openapi.yml
  format: yaml
  label: Pliant Organizations API
  slug: pliant-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-organizations-api-openapi.yml
- filename: pliant-payments-api-openapi.yml
  format: yaml
  label: Pliant Payments API
  slug: pliant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-payments-api-openapi.yml
- filename: pliant-receipt-automatching-api-openapi.yml
  format: yaml
  label: Pliant Receipt Automatching API
  slug: pliant-receipt-automatching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-receipt-automatching-api-openapi.yml
- filename: pliant-receipts-api-openapi.yml
  format: yaml
  label: Pliant Receipts API
  slug: pliant-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-receipts-api-openapi.yml
- filename: pliant-statements-api-openapi.yml
  format: yaml
  label: Pliant Statements API
  slug: pliant-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-statements-api-openapi.yml
- filename: pliant-test-data-generator-sandbox-only-api-openapi.yml
  format: yaml
  label: Pliant Test Data Generator (Sandbox-only) API
  slug: pliant-test-data-generator-sandbox-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-test-data-generator-sandbox-only-api-openapi.yml
- filename: pliant-transactions-api-openapi.yml
  format: yaml
  label: Pliant Transactions API
  slug: pliant-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-transactions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pliant Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pliant secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pliant
provider_slug: pliant
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials flow. During onboarding the customer receives a clientId and clientSecret, which are exchanged at the Auth0 token endpoint (separate production and sandbox endpoints) with grant_type=client_credentials for an access_token. The bearer access token must be included in the Authorization header on every API request. Tokens expire (e.g. expires_in 86400 = 24h). The authorization flow must be handled exclusively by a secure backend; web frontends and mobile apps must not call the API directly or expose the clientSecret.
  flow: clientCredentials
  in: header
  name: OAuth2ClientCredentials
  parameter_name: Authorization
  type: oauth2
slug: pliant-authentication
source_filename: pliant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://customer-api.getpliant.com/docs/authenticated-api-usage\ndocs: https://customer-api.getpliant.com/docs/authenticated-api-usage\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\n  identity_provider: Auth0\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    OAuth 2.0 Client Credentials flow. During onboarding the customer receives a\n    clientId and clientSecret, which are exchanged at the Auth0 token endpoint\n    (separate production and sandbox endpoints) with grant_type=client_credentials\n    for an access_token. The bearer access token must be included in the\n    Authorization header on every API request. Tokens expire (e.g. expires_in\n    86400 = 24h). The authorization flow must be handled exclusively by a secure\n    backend; web frontends and mobile apps must not call the API directly or\n    expose the clientSecret.\n\
  \  in: header\n  parameter_name: Authorization\nscopes_documented: false\nscopes_note: >-\n  The Pro API does not document OAuth scopes/permissions; access is scoped by the\n  onboarded client credentials rather than per-request scope grants.\ncallback_authentication: >-\n  Inbound callbacks (webhooks) can be verified via Ed25519 signature headers, and\n  Pliant can optionally deliver callbacks with OAuth 2.0 authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/authentication/pliant-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Payments
- Corporate Cards
- Card Issuing
- Spend Management
- Expense Management
- Fintech
- Cards-as-a-Service
- Banking as a Service
- Travel
- Accounting
---
