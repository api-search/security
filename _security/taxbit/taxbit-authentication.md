---
api_key_in: []
auth_types: []
description: 'The TaxBit APIs authenticate every request with a bearer token. Two token scopes exist: a tenant-scoped bearer token (the primary mechanism) and an account-owner-scoped bearer token used for tax-documentation (W-8/W-9) flows. The tenant-scoped token is obtained by POSTing OAuth-style credentials (client_id, client_secret, tenant_id) from the Taxbit Dashboard Developer Settings; it is valid for 24 hours.'
kind: authentication
layout: security
method: searched
name: Taxbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: TaxBit declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TaxBit
provider_slug: taxbit
scheme_count: 2
schemes:
- covers:
  - Account Owners
  - Accounts
  - Transactions
  - Assets
  - Documents
  - Form Items
  - Gains
  - Inventory
  - Reports
  - Filers
  - Disposition Methods
  - Transfer Lots
  - Tax Treaty Rates
  - Real-Time TIN Validation
  description: 'Primary authorization mechanism. Exchange client credentials for a tenant-scoped bearer token, valid for 24 hours, then send it as Authorization: Bearer <token> on API requests.'
  id: tenant_scoped_bearer_token
  lifetime: 24 hours
  mint_endpoint: post_oauth-token
  mint_url: https://apidocs.taxbit.com/reference/post_oauth-token
  primary: true
  scheme: bearer
  type: http
- covers:
  - Account Owners
  - Tax Documentation
  description: Authorizes submitting and accessing Tax Documentation on behalf of a specific account owner. Designed for the W-8/W-9 solution and the embedded Tax Documentation SDK (see components/taxbit-components.yml). Handle token expiration per https://apidocs.taxbit.com/docs/handling-token-expiration.
  id: account_owner_scoped_bearer_token
  mint_endpoint: post_oauth-account-owner-token
  mint_url: https://apidocs.taxbit.com/reference/post_oauth-account-owner-token
  primary: false
  scheme: bearer
  type: http
slug: taxbit-authentication
source_filename: taxbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://apidocs.taxbit.com/reference/auth-token,\n  https://apidocs.taxbit.com/reference/post_oauth-token,\n  https://apidocs.taxbit.com/reference/post_oauth-account-owner-token, and\n  https://apidocs.taxbit.com/docs/accessing-the-api. The OpenAPI spec is served\n  by ReadMe behind auth and could not be downloaded, so this profile is built\n  from the published auth documentation rather than derived from securitySchemes.\ndescription: >-\n  The TaxBit APIs authenticate every request with a bearer token. Two token\n  scopes exist: a tenant-scoped bearer token (the primary mechanism) and an\n  account-owner-scoped bearer token used for tax-documentation (W-8/W-9) flows.\n  The tenant-scoped token is obtained by POSTing OAuth-style credentials\n  (client_id, client_secret, tenant_id) from the Taxbit Dashboard Developer\n  Settings; it is valid for 24 hours.\ntype: bearer\napi_host_pattern: https://api.<environment>.enterprise.taxbit.com\n\
  api_host_examples:\n  - https://api.multi1.enterprise.taxbit.com\n  - https://api.eutax1.enterprise.taxbit.com\ncredentials:\n  fields: [client_id, client_secret, tenant_id]\n  source: Taxbit Dashboard — Developer Settings page\nschemes:\n  - id: tenant_scoped_bearer_token\n    type: http\n    scheme: bearer\n    primary: true\n    mint_endpoint: post_oauth-token\n    mint_url: https://apidocs.taxbit.com/reference/post_oauth-token\n    lifetime: 24 hours\n    covers:\n      - Account Owners\n      - Accounts\n      - Transactions\n      - Assets\n      - Documents\n      - Form Items\n      - Gains\n      - Inventory\n      - Reports\n      - Filers\n      - Disposition Methods\n      - Transfer Lots\n      - Tax Treaty Rates\n      - Real-Time TIN Validation\n    description: >-\n      Primary authorization mechanism. Exchange client credentials for a\n      tenant-scoped bearer token, valid for 24 hours, then send it as\n      Authorization: Bearer <token> on API requests.\n  - id: account_owner_scoped_bearer_token\n\
  \    type: http\n    scheme: bearer\n    primary: false\n    mint_endpoint: post_oauth-account-owner-token\n    mint_url: https://apidocs.taxbit.com/reference/post_oauth-account-owner-token\n    covers:\n      - Account Owners\n      - Tax Documentation\n    description: >-\n      Authorizes submitting and accessing Tax Documentation on behalf of a\n      specific account owner. Designed for the W-8/W-9 solution and the embedded\n      Tax Documentation SDK (see components/taxbit-components.yml). Handle token\n      expiration per https://apidocs.taxbit.com/docs/handling-token-expiration.\ndocs:\n  overview: https://apidocs.taxbit.com/reference/auth-token\n  accessing_the_api: https://apidocs.taxbit.com/docs/accessing-the-api\n  token_expiration: https://apidocs.taxbit.com/docs/handling-token-expiration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taxbit/refs/heads/main/authentication/taxbit-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Tax
- Tax Compliance
- Information Reporting
- Digital Assets
- Cryptocurrency
- Accounting
- Regtech
---
