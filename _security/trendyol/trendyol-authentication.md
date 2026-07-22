---
api_key_in: []
auth_types:
- http
- oauth2
description: How a caller authenticates to the Trendyol Marketplace / Partner API. Sellers and self-integrators use HTTP Basic authentication with credentials generated in the Seller Center; integrators managing many suppliers use an OAuth 2.0 authorization-code flow. Every request must also carry a User-Agent header or it is rejected with 403.
kind: authentication
layout: security
method: searched
name: Trendyol Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Trendyol secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Trendyol
provider_slug: trendyol
scheme_count: 3
schemes:
- credentials:
  - supplierId (a.k.a. sellerId) — carried in the URL path
  - API Key
  - API Secret Key
  credentials_source: Seller Center → "Hesap Bilgileri / Entegrasyon Bilgileri" (Account Details → Integration Information). Visible only to the seller panel master user.
  description: 'HTTP Basic authentication. The credential is base64(API Key : API Secret Key). The supplierId / sellerId is carried in the request path (…/sellers/{sellerId}/…), not in the credential. Credentials are unique per supplierId and differ between the production and stage (test) environments.'
  docs: https://developers.trendyol.com/docs/2-authorization
  header_example: 'Authorization: Basic <base64(apiKey:apiSecret)>'
  name: basicAuth
  scheme: basic
  type: http
- description: Every request to the Partner API must send a User-Agent header or it is rejected with HTTP 403. Format is "{sellerId} - {CompanyName}" (alphanumeric, max 30 chars) when working through an integrator company, or "{sellerId} - SelfIntegration" when self-integrated.
  header_example: 'User-Agent: 1234 - SelfIntegration'
  name: userAgent
  required: true
  type: header
- description: 'For integrators that manage many suppliers, Trendyol offers an OAuth 2.0 authorization-code flow: the integrator registers a client_id / client_secret, each supplier authorizes the integrator from the Partner panel, and the integrator receives a ~1 hour access token plus a ~30 day refresh token. Applies to integrator platforms rather than single-seller self-integrations.'
  docs: https://developers.trendyol.com/docs/2-authorization
  flows:
  - access_token_ttl: ~1 hour
    flow: authorizationCode
    refresh_token_ttl: ~30 days
  name: oauth2
  type: oauth2
slug: trendyol-authentication
source_filename: trendyol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://developers.trendyol.com/docs/2-authorization and\n  https://developers.trendyol.com/v2.0/docs/authorization — the Trendyol\n  Marketplace (Partner) API authorization documentation. Trendyol does not\n  publish a single OpenAPI document (endpoints are embedded per-page in the\n  ReadMe docs / llms.txt index), so this profile is captured from the docs\n  rather than derived from a spec.\ndescription: >-\n  How a caller authenticates to the Trendyol Marketplace / Partner API. Sellers\n  and self-integrators use HTTP Basic authentication with credentials generated\n  in the Seller Center; integrators managing many suppliers use an OAuth 2.0\n  authorization-code flow. Every request must also carry a User-Agent header or\n  it is rejected with 403.\nsummary:\n  types: [http, oauth2]\n  http_scheme: basic\n  oauth2_flows: [authorizationCode]\n  mandatory_headers: [Authorization, User-Agent]\nschemes:\n  - name: basicAuth\n\
  \    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication. The credential is base64(API Key : API Secret\n      Key). The supplierId / sellerId is carried in the request path\n      (…/sellers/{sellerId}/…), not in the credential. Credentials are unique\n      per supplierId and differ between the production and stage (test)\n      environments.\n    credentials:\n      - supplierId (a.k.a. sellerId) — carried in the URL path\n      - API Key\n      - API Secret Key\n    credentials_source: >-\n      Seller Center → \"Hesap Bilgileri / Entegrasyon Bilgileri\" (Account\n      Details → Integration Information). Visible only to the seller panel\n      master user.\n    header_example: 'Authorization: Basic <base64(apiKey:apiSecret)>'\n    docs: https://developers.trendyol.com/docs/2-authorization\n  - name: userAgent\n    type: header\n    required: true\n    description: >-\n      Every request to the Partner API must send a User-Agent header or it is\n  \
  \    rejected with HTTP 403. Format is \"{sellerId} - {CompanyName}\"\n      (alphanumeric, max 30 chars) when working through an integrator company,\n      or \"{sellerId} - SelfIntegration\" when self-integrated.\n    header_example: 'User-Agent: 1234 - SelfIntegration'\n  - name: oauth2\n    type: oauth2\n    description: >-\n      For integrators that manage many suppliers, Trendyol offers an OAuth 2.0\n      authorization-code flow: the integrator registers a client_id /\n      client_secret, each supplier authorizes the integrator from the Partner\n      panel, and the integrator receives a ~1 hour access token plus a ~30 day\n      refresh token. Applies to integrator platforms rather than single-seller\n      self-integrations.\n    flows:\n      - flow: authorizationCode\n        access_token_ttl: ~1 hour\n        refresh_token_ttl: ~30 days\n    docs: https://developers.trendyol.com/docs/2-authorization\nerrors:\n  - status: 401\n    exception: ClientApiAuthenticationException\n\
  \    cause: Missing or incorrect Basic credentials.\n  - status: 403\n    cause: Missing User-Agent header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trendyol/refs/heads/main/authentication/trendyol-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Ecommerce
- Marketplace
- Retail
- Fashion
- Turkey
- Order Management
- Fulfillment
- Logistics
- Webhooks
---
