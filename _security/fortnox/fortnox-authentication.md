---
api_key_in: []
api_specs:
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Invoices API
  slug: fortnox-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Customers API
  slug: fortnox-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Articles API
  slug: fortnox-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Orders API
  slug: fortnox-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Offers API
  slug: fortnox-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Bookkeeping API
  slug: fortnox-bookkeeping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Suppliers & Supplier Invoices API
  slug: fortnox-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-openapi.yml
  format: yaml
  label: Fortnox Projects API
  slug: fortnox-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/openapi/fortnox-openapi.yml
- filename: fortnox-asyncapi.yml
  format: yaml
  label: Fortnox Topics WebSocket API
  slug: fortnox-topics-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/asyncapi/fortnox-asyncapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: documented
name: Fortnox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fortnox secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fortnox
provider_slug: fortnox
scheme_count: 3
schemes:
- authorizationUrl: https://apps.fortnox.se/oauth-v1/auth
  description: Fortnox uses OAuth2 Authorization Code Flow. The end customer authorizes your registered developer application; you exchange the Authorization-Code (valid 10 minutes) for an Access-Token (Bearer JWT, valid 1 hour) and a Refresh-Token (valid 45 days). Refreshing rotates the Refresh-Token. The legacy fixed Access-Token / Client-Secret integration-key model was fully deprecated on 2025-04-30.
  flow: authorizationCode
  name: oauth2AuthorizationCode
  sources:
  - https://www.fortnox.se/developer/authorization
  - https://www.fortnox.se/developer/authorization/get-access-token
  tokenLifetimes:
    accessToken: 1 hour
    authorizationCode: 10 minutes
    refreshToken: 45 days
  tokenUrl: https://apps.fortnox.se/oauth-v1/token
  type: oauth2
- description: On every REST call the OAuth2 Access-Token (Bearer JWT) is sent in the Access-Token request header.
  headerName: Access-Token
  in: header
  name: accessTokenHeader
  sources:
  - https://www.fortnox.se/developer/authorization
  type: apiKey
- description: On every REST call the Client-Secret issued to your Fortnox developer application is sent in the Client-Secret request header, alongside the Access-Token header.
  headerName: Client-Secret
  in: header
  name: clientSecretHeader
  sources:
  - https://www.fortnox.se/developer/authorization
  type: apiKey
slug: fortnox-authentication
source_filename: fortnox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://www.fortnox.se/developer/authorization\nprovider: Fortnox\nproviderId: fortnox\nsummary:\n  types:\n  - oauth2\n  - apiKey\nschemes:\n- name: oauth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://apps.fortnox.se/oauth-v1/auth\n  tokenUrl: https://apps.fortnox.se/oauth-v1/token\n  description: >-\n    Fortnox uses OAuth2 Authorization Code Flow. The end customer authorizes\n    your registered developer application; you exchange the Authorization-Code\n    (valid 10 minutes) for an Access-Token (Bearer JWT, valid 1 hour) and a\n    Refresh-Token (valid 45 days). Refreshing rotates the Refresh-Token. The\n    legacy fixed Access-Token / Client-Secret integration-key model was fully\n    deprecated on 2025-04-30.\n  tokenLifetimes:\n    authorizationCode: 10 minutes\n    accessToken: 1 hour\n    refreshToken: 45 days\n  sources:\n  - https://www.fortnox.se/developer/authorization\n\
  \  - https://www.fortnox.se/developer/authorization/get-access-token\n- name: accessTokenHeader\n  type: apiKey\n  in: header\n  headerName: Access-Token\n  description: >-\n    On every REST call the OAuth2 Access-Token (Bearer JWT) is sent in the\n    Access-Token request header.\n  sources:\n  - https://www.fortnox.se/developer/authorization\n- name: clientSecretHeader\n  type: apiKey\n  in: header\n  headerName: Client-Secret\n  description: >-\n    On every REST call the Client-Secret issued to your Fortnox developer\n    application is sent in the Client-Secret request header, alongside the\n    Access-Token header.\n  sources:\n  - https://www.fortnox.se/developer/authorization\nnotes: >-\n  Scopes are granted per Fortnox resource area (e.g. invoice, customer, article,\n  order, offer, bookkeeping, supplier, supplierinvoice, project) and requested\n  during the authorization step. The WebSocket Topics API\n  (wss://ws.fortnox.se/topics-v1) authenticates by sending the Client-Secret\
  \ and\n  per-tenant Access-Tokens inside the add-tenants-v1 command after the socket\n  opens, rather than via request headers.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortnox/refs/heads/main/authentication/fortnox-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Accounting
- ERP
- Invoicing
- Bookkeeping
- Sweden
- Nordics
- Finance
- Vouchers
- Customers
- SaaS
---
