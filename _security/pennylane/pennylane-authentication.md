---
api_key_in: []
api_specs:
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Customer Invoicing API
  slug: pennylane-customer-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Supplier Invoicing API
  slug: pennylane-supplier-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Accounting & Ledger API
  slug: pennylane-accounting-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Accounting Exports API
  slug: pennylane-accounting-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Banking API
  slug: pennylane-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Customers & Suppliers API
  slug: pennylane-customers-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Products Catalog API
  slug: pennylane-products-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Quotes API
  slug: pennylane-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Billing Subscriptions API
  slug: pennylane-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Direct Debit Mandates API
  slug: pennylane-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Change Events API
  slug: pennylane-change-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane E-Invoicing (Plateforme Agréée) API
  slug: pennylane-einvoicing-pa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
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
