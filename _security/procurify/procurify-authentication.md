---
api_key_in:
- cookie
api_specs:
- filename: procurify-account-codes-api-openapi.yml
  format: yaml
  label: Procurify account-codes API
  slug: procurify-account-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-account-codes-api-openapi.yml
- filename: procurify-accounts-api-openapi.yml
  format: yaml
  label: Procurify accounts API
  slug: procurify-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-accounts-api-openapi.yml
- filename: procurify-ap-api-openapi.yml
  format: yaml
  label: Procurify ap API
  slug: procurify-ap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-ap-api-openapi.yml
- filename: procurify-catalog-api-openapi.yml
  format: yaml
  label: Procurify catalog API
  slug: procurify-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-catalog-api-openapi.yml
- filename: procurify-currencies-api-openapi.yml
  format: yaml
  label: Procurify currencies API
  slug: procurify-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-currencies-api-openapi.yml
- filename: procurify-custom-fields-api-openapi.yml
  format: yaml
  label: Procurify custom-fields API
  slug: procurify-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-custom-fields-api-openapi.yml
- filename: procurify-departments-api-openapi.yml
  format: yaml
  label: Procurify departments API
  slug: procurify-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-departments-api-openapi.yml
- filename: procurify-locations-api-openapi.yml
  format: yaml
  label: Procurify locations API
  slug: procurify-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-locations-api-openapi.yml
- filename: procurify-oauth-api-openapi.yml
  format: yaml
  label: Procurify oauth API
  slug: procurify-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-oauth-api-openapi.yml
- filename: procurify-order-items-api-openapi.yml
  format: yaml
  label: Procurify order-items API
  slug: procurify-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-order-items-api-openapi.yml
- filename: procurify-permissions-api-openapi.yml
  format: yaml
  label: Procurify permissions API
  slug: procurify-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-permissions-api-openapi.yml
- filename: procurify-public-api-openapi.yml
  format: yaml
  label: Procurify public API
  slug: procurify-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-public-api-openapi.yml
- filename: procurify-purchase-orders-api-openapi.yml
  format: yaml
  label: Procurify purchase-orders API
  slug: procurify-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-purchase-orders-api-openapi.yml
- filename: procurify-receipt-api-openapi.yml
  format: yaml
  label: Procurify receipt API
  slug: procurify-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-receipt-api-openapi.yml
- filename: procurify-requisitions-api-openapi.yml
  format: yaml
  label: Procurify requisitions API
  slug: procurify-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-requisitions-api-openapi.yml
- filename: procurify-users-api-openapi.yml
  format: yaml
  label: Procurify users API
  slug: procurify-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-users-api-openapi.yml
- filename: procurify-vendors-api-openapi.yml
  format: yaml
  label: Procurify vendors API
  slug: procurify-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-vendors-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Procurify Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Procurify secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Procurify
provider_slug: procurify
scheme_count: 4
schemes:
- name: BasicAuthentication
  scheme: basic
  sources:
  - openapi/procurify-procurify-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: M2MAuthentication
  scheme: bearer
  sources:
  - openapi/procurify-procurify-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://<your-domain>.procurify.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://<your-domain>.procurify.com/oauth/token
  name: RemoteAuthentication
  sources:
  - openapi/procurify-procurify-api-openapi.yml
  type: oauth2
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/procurify-procurify-api-openapi.yml
  type: apiKey
slug: procurify-authentication
source_filename: procurify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/procurify-procurify-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BasicAuthentication\n  type: http\n  scheme: basic\n  sources:\n  - openapi/procurify-procurify-api-openapi.yml\n- name: M2MAuthentication\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/procurify-procurify-api-openapi.yml\n- name: RemoteAuthentication\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://<your-domain>.procurify.com/oauth/authorize\n    tokenUrl: https://<your-domain>.procurify.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/procurify-procurify-api-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/procurify-procurify-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/authentication/procurify-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Spend Management
- Procurement
- Purchase Orders
- Accounts Payable
- Vendor Management
- Budget Tracking
- Procure-to-Pay
- ERP Integration
---
