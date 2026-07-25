---
api_key_in: []
api_specs:
- filename: pennylane-account-api-openapi.yml
  format: yaml
  label: Pennylane Account API
  slug: pennylane-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-account-api-openapi.yml
- filename: pennylane-accounting-exports-api-openapi.yml
  format: yaml
  label: Pennylane Accounting Exports API
  slug: pennylane-accounting-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-accounting-exports-api-openapi.yml
- filename: pennylane-bank-accounts-api-openapi.yml
  format: yaml
  label: Pennylane Bank Accounts API
  slug: pennylane-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-bank-accounts-api-openapi.yml
- filename: pennylane-billing-subscriptions-api-openapi.yml
  format: yaml
  label: Pennylane Billing Subscriptions API
  slug: pennylane-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-billing-subscriptions-api-openapi.yml
- filename: pennylane-categories-api-openapi.yml
  format: yaml
  label: Pennylane Categories API
  slug: pennylane-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-categories-api-openapi.yml
- filename: pennylane-change-events-api-openapi.yml
  format: yaml
  label: Pennylane Change Events API
  slug: pennylane-change-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-change-events-api-openapi.yml
- filename: pennylane-customer-invoices-api-openapi.yml
  format: yaml
  label: Pennylane Customer Invoices API
  slug: pennylane-customer-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-customer-invoices-api-openapi.yml
- filename: pennylane-customers-api-openapi.yml
  format: yaml
  label: Pennylane Customers API
  slug: pennylane-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-customers-api-openapi.yml
- filename: pennylane-e-invoicing-api-openapi.yml
  format: yaml
  label: Pennylane E-Invoicing API
  slug: pennylane-e-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-e-invoicing-api-openapi.yml
- filename: pennylane-file-attachments-api-openapi.yml
  format: yaml
  label: Pennylane File Attachments API
  slug: pennylane-file-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-file-attachments-api-openapi.yml
- filename: pennylane-journals-api-openapi.yml
  format: yaml
  label: Pennylane Journals API
  slug: pennylane-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-journals-api-openapi.yml
- filename: pennylane-ledger-accounts-api-openapi.yml
  format: yaml
  label: Pennylane Ledger Accounts API
  slug: pennylane-ledger-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-ledger-accounts-api-openapi.yml
- filename: pennylane-ledger-entries-api-openapi.yml
  format: yaml
  label: Pennylane Ledger Entries API
  slug: pennylane-ledger-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-ledger-entries-api-openapi.yml
- filename: pennylane-mandates-api-openapi.yml
  format: yaml
  label: Pennylane Mandates API
  slug: pennylane-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-mandates-api-openapi.yml
- filename: pennylane-products-api-openapi.yml
  format: yaml
  label: Pennylane Products API
  slug: pennylane-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-products-api-openapi.yml
- filename: pennylane-quotes-api-openapi.yml
  format: yaml
  label: Pennylane Quotes API
  slug: pennylane-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-quotes-api-openapi.yml
- filename: pennylane-supplier-invoices-api-openapi.yml
  format: yaml
  label: Pennylane Supplier Invoices API
  slug: pennylane-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-supplier-invoices-api-openapi.yml
- filename: pennylane-suppliers-api-openapi.yml
  format: yaml
  label: Pennylane Suppliers API
  slug: pennylane-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-suppliers-api-openapi.yml
- filename: pennylane-transactions-api-openapi.yml
  format: yaml
  label: Pennylane Transactions API
  slug: pennylane-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-transactions-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pennylane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pennylane secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pennylane
provider_slug: pennylane
scheme_count: 2
schemes:
- bearerFormat: token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pennylane-openapi.yml
  - https://pennylane.readme.io/docs/getting-started
  type: http
- authorizationUrl: https://app.pennylane.com/oauth/authorize
  flow: authorizationCode
  name: oauth2
  revocationUrl: https://app.pennylane.com/oauth/revoke
  sources:
  - https://pennylane.readme.io/docs/oauth-20-walkthrough
  tokenUrl: https://app.pennylane.com/oauth/token
  type: oauth2
slug: pennylane-authentication
source_filename: pennylane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/pennylane-openapi.yml\ndocs: https://pennylane.readme.io/docs/oauth-20-walkthrough\nsummary:\n  types:\n  - http\n  - oauth2\nnotes: >-\n  Pennylane API v2 requires a Bearer token in the Authorization header on every\n  request. The token can be a Company API token (generated in company account\n  settings), a Firm API token (generated in firm account settings), or an\n  OAuth 2.0 access token for integration partners. OAuth apps are registered via\n  the Pennylane Partnerships team; the authorization code grant is used with\n  refresh tokens. Scopes follow a resource:readonly / resource:all pattern and\n  enforce least privilege (403 Forbidden when a required scope is missing).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  sources:\n  - openapi/pennylane-openapi.yml\n  - https://pennylane.readme.io/docs/getting-started\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n\
  \  authorizationUrl: https://app.pennylane.com/oauth/authorize\n  tokenUrl: https://app.pennylane.com/oauth/token\n  revocationUrl: https://app.pennylane.com/oauth/revoke\n  sources:\n  - https://pennylane.readme.io/docs/oauth-20-walkthrough\ntokenContexts:\n- name: Company API Token\n  description: Generated in a company's Pennylane account settings; scoped to that company.\n- name: Firm API Token\n  description: Generated in a firm's account settings; can access resources across managed client companies, filtered by the granting user's permissions.\n- name: OAuth 2.0\n  description: For integration partners; authorization code grant with refresh tokens, per-company or per-firm consent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/authentication/pennylane-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Accounting
- Invoicing
- Fintech
- Financial Data
- Banking
- France
- SME
---
