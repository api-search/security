---
anonymous_access: false
api_key_in: []
api_specs:
- filename: postman_collection.quickstreamapi.json
  format: json
  label: Westpac QuickStream REST API
  slug: westpac-quickstream-rest-api
  spec_type: Postman
  url: https://quickstream.westpac.com.au/docs/downloads/postman_collection.quickstreamapi.json
- filename: westpac-banking-account-balances-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Balances API
  slug: westpac-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-balances-api-openapi.yml
- filename: westpac-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Direct Debits API
  slug: westpac-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-direct-debits-api-openapi.yml
- filename: westpac-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Scheduled Payments API
  slug: westpac-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-scheduled-payments-api-openapi.yml
- filename: westpac-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Transactions API
  slug: westpac-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-transactions-api-openapi.yml
- filename: westpac-banking-accounts-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Accounts API
  slug: westpac-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-accounts-api-openapi.yml
- filename: westpac-banking-payees-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Payees API
  slug: westpac-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-payees-api-openapi.yml
- filename: westpac-banking-products-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Products API
  slug: westpac-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-products-api-openapi.yml
auth_types:
- http-basic
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Westpac Authentication
name_suffix: Authentication
oauth_flows: []
overview: Westpac secures its APIs with http-basic across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Westpac
provider_slug: westpac
scheme_count: 1
schemes:
- api: QuickStream REST API v1
  credentials:
  - detail: allows you to process payments and provides full access to the API.
    name: Secret API Key
  - detail: can be used in mobile applications and web pages and has limited access.
    name: Publishable API Key
  detail: Authentication to the API is via HTTP Basic Auth. You must send an API key as the Basic Authentication username. Leave the password blank.
  docs:
  - https://quickstream.westpac.com.au/docs/quickstreamapi/v1/
  - https://quickstream.westpac.com.au/docs/quickstreamapi/v1/api-keys
  errors:
    '401': Sending an invalid API key returns a 401 Unauthorized HTTP status code.
    '403': Sending a valid API key, but the wrong type of key for the resource returns a 403 Forbidden HTTP status code.
  id: quickstream-basic
  key_lifetime: Secret API keys expire after 2 years and then you must use a new key.
  rotation: GET /api-keys/latest returns the secret key to use from now on; the docs say "You should do this once per day."
  scheme: basic
  type: http
slug: westpac-authentication
source_filename: westpac-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: https://quickstream.westpac.com.au/docs/quickstreamapi/v1/\ndocs: https://www.westpac.com.au/about-westpac/innovation/open-banking/product-api/\nsummary:\n  types:\n  - http-basic\n  api_key_in: []\n  oauth2_flows: []\n  note: CDR Product Reference Data (listBankingProducts, getBankingProductDetail) is unauthenticated;\n    the CDR contract declares no securitySchemes. Consumer-data CDR endpoints are reached only through\n    the CDR ADR consent flow (see scopes/westpac-scopes.yml). Westpac's own QuickStream REST API uses\n    HTTP Basic Auth with a Secret or Publishable API key as the username.\nschemes:\n- id: quickstream-basic\n  api: QuickStream REST API v1\n  type: http\n  scheme: basic\n  detail: Authentication to the API is via HTTP Basic Auth. You must send an API key as the Basic Authentication\n    username. Leave the password blank.\n  credentials:\n  - name: Secret API Key\n    detail: allows you to process payments\
  \ and provides full access to the API.\n  - name: Publishable API Key\n    detail: can be used in mobile applications and web pages and has limited access.\n  key_lifetime: Secret API keys expire after 2 years and then you must use a new key.\n  rotation: GET /api-keys/latest returns the secret key to use from now on; the docs say \"You should do\n    this once per day.\"\n  errors:\n    '401': Sending an invalid API key returns a 401 Unauthorized HTTP status code.\n    '403': Sending a valid API key, but the wrong type of key for the resource returns a 403 Forbidden\n      HTTP status code.\n  docs:\n  - https://quickstream.westpac.com.au/docs/quickstreamapi/v1/\n  - https://quickstream.westpac.com.au/docs/quickstreamapi/v1/api-keys\npublic_access:\n  authenticated: false\n  detail: listProducts and getProductDetail are open, unauthenticated GET endpoints.\nconsumer_data_sharing:\n  detail: Access to consumer/account data beyond product reference data is NOT available through this\n \
  \   public API. It flows through the CDR's Accredited Data Recipient (ADR) model, which uses an OAuth\n    2.0 / OpenID Connect, FAPI-hardened consent flow operated through the CDR ecosystem (accreditation\n    + the CDR Register), not a Westpac-issued developer credential. That surface is out of scope for this\n    public PRD contract.\nderived_from: openapi/_original/westpac-cds-banking-openapi.yml\ndocs_quickstream: https://quickstream.westpac.com.au/docs/quickstreamapi/v1/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/authentication/westpac-authentication.yml
summary_line: http-basic · 1 scheme
tags:
- Finance
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
