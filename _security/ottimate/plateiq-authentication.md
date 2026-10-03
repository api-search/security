---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ottimate-accounts-api-openapi.yml
  format: yaml
  label: Ottimate Accounts API
  slug: ottimate-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-accounts-api-openapi.yml
- filename: ottimate-batch-api-openapi.yml
  format: yaml
  label: Ottimate Batch API
  slug: ottimate-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-batch-api-openapi.yml
- filename: ottimate-catalog-api-openapi.yml
  format: yaml
  label: Ottimate Catalog API
  slug: ottimate-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-catalog-api-openapi.yml
- filename: ottimate-dimensions-api-openapi.yml
  format: yaml
  label: Ottimate Dimensions API
  slug: ottimate-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-dimensions-api-openapi.yml
- filename: ottimate-invoices-api-openapi.yml
  format: yaml
  label: Ottimate Invoices API
  slug: ottimate-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-invoices-api-openapi.yml
- filename: ottimate-oauth-api-openapi.yml
  format: yaml
  label: Ottimate OAuth API
  slug: ottimate-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-oauth-api-openapi.yml
- filename: ottimate-receipts-api-openapi.yml
  format: yaml
  label: Ottimate Receipts API
  slug: ottimate-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-receipts-api-openapi.yml
- filename: ottimate-vendors-api-openapi.yml
  format: yaml
  label: Ottimate Vendors API
  slug: ottimate-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-vendors-api-openapi.yml
- filename: ottimate-purchase-orders-api-openapi.yml
  format: yaml
  label: Ottimate Purchase Orders API
  slug: ottimate-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-purchase-orders-api-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Plateiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ottimate secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ottimate
provider_slug: ottimate
scheme_count: 2
schemes:
- description: Server-to-server OAuth2 client-credentials flow. Client ID and Client Secret are provisioned by an Ottimate Partner Manager. Tokens should be cached and refreshed on expiry or on a 401 response.
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2
  parameters:
  - client_id
  - client_secret
  - grant_type
  - scope
  scheme: bearer
  scopes:
  - accounts.can_access_dashboard
  token_lifetime_seconds_example: 31536000
  token_url_production: https://api.ottimate.com/v1/oauth/token
  token_url_sandbox: https://sandbox-auth.ottimate.com/oauth/token
  type: oauth2
- description: Per-client-account API key, required on every request in addition to the Bearer token. Provisioned by an Ottimate Partner Manager. Rotating the API key invalidates all cached idempotency entries scoped to the old key.
  header_name: X-API-Key
  in: header
  name: ApiKey
  type: apiKey
slug: plateiq-authentication
source_filename: plateiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.ottimate.com/auth.md\ndocs: https://docs.ottimate.com/auth\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  notes: >-\n    Every request to the Ottimate API requires BOTH an `X-API-Key` header and an\n    `Authorization: Bearer <access_token>` header. The access token is obtained\n    via the OAuth2 client-credentials flow; the API key is provisioned per client\n    account by an Ottimate Partner Manager.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: clientCredentials\n  scheme: bearer\n  token_url_production: https://api.ottimate.com/v1/oauth/token\n  token_url_sandbox: https://sandbox-auth.ottimate.com/oauth/token\n  grant_type: client_credentials\n  parameters:\n  - client_id\n  - client_secret\n  - grant_type\n  - scope\n  scopes:\n  - accounts.can_access_dashboard\n  token_lifetime_seconds_example: 31536000\n  description: >-\n    Server-to-server OAuth2 client-credentials flow. Client ID and Client Secret\n\
  \    are provisioned by an Ottimate Partner Manager. Tokens should be cached and\n    refreshed on expiry or on a 401 response.\n- name: ApiKey\n  type: apiKey\n  in: header\n  header_name: X-API-Key\n  description: >-\n    Per-client-account API key, required on every request in addition to the\n    Bearer token. Provisioned by an Ottimate Partner Manager. Rotating the API\n    key invalidates all cached idempotency entries scoped to the old key.\naccess_control:\n  model: OAuth app -> API User -> scoped data access\n  scope_levels:\n  - account-level    # all companies and locations in the account\n  - company-level    # single company and all its locations\n  - location-level   # specific location(s) only\n  docs: https://docs.ottimate.com/account-structure/scoping\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/authentication/plateiq-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Enterprise Saas
- Accounts Payable
- Invoice Automation
- Payments
- Fintech
- Restaurant
- Procurement
- Spend Management
- ERP Integration
---
