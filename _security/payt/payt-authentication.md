---
api_key_in: []
api_specs:
- filename: payt-openapi-original.json
  format: json
  label: Payt Customer API v1
  slug: payt-customer-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payt/refs/heads/main/openapi/payt-openapi-original.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Payt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Payt secures its APIs with oauth2 and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Payt
provider_slug: payt
scheme_count: 4
schemes:
- description: 'OAuth 2.0 access token or static API token, sent as Authorization: Bearer <token> on almost all endpoints.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/payt-openapi-original.json
  - https://docs.paytsoftware.com/authentication/tokens
  type: http
- authorizationUrl: https://app.paytsoftware.com/oauth/authorize
  description: OAuth 2.0 Authorization Code flow. The user authorizes an application, selecting which administrations to grant and which scopes (permissions) to allow. The authorization code expires after 10 minutes; access tokens live 2 hours and are renewed with a rotating refresh token that lasts 90 days from last use.
  flow: authorizationCode
  name: oauth2_authorization_code
  refresh: true
  sources:
  - https://docs.paytsoftware.com/authentication/authorization
  - https://docs.paytsoftware.com/authentication/tokens
  tokenUrl: https://api.paytsoftware.com/oauth/token
  type: oauth2
- description: HTTP Basic (base64 client_id:client_secret, RFC 4648) is required only on the token endpoints (/oauth/token) and the sign_up endpoint - used to obtain or refresh tokens, not to call resource endpoints.
  name: basic_client_credentials
  scheme: basic
  sources:
  - https://docs.paytsoftware.com/authentication/basic-authorization
  type: http
- description: Static API token fallback for clients unable to implement OAuth 2.0. Presented as a Bearer token like an OAuth access token. Documented as the less-secure option.
  name: static_api_token
  scheme: bearer
  sources:
  - https://docs.paytsoftware.com/authentication/authorization
  type: http
slug: payt-authentication
source_filename: payt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.paytsoftware.com/authentication/authorization\ndocs: https://docs.paytsoftware.com/authentication/authorization\nsummary:\n  types:\n  - oauth2\n  - http\n  primary: oauth2\n  notes: >-\n    Payt authorizes API requests with an OAuth 2.0 Authorization Code flow (the\n    recommended path) or, as a less-secure fallback, a static API token. In both\n    cases the resulting access token is presented as an HTTP Bearer token. The\n    OpenAPI declares only the bearerAuth HTTP bearer scheme; the OAuth 2.0\n    machinery (authorize + token endpoints, scopes, refresh tokens) is documented\n    in the auth guide rather than the spec.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    OAuth 2.0 access token or static API token, sent as Authorization: Bearer <token>\n    on almost all endpoints.\n  sources:\n  - openapi/payt-openapi-original.json\n  - https://docs.paytsoftware.com/authentication/tokens\n\
  - name: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://app.paytsoftware.com/oauth/authorize\n  tokenUrl: https://api.paytsoftware.com/oauth/token\n  refresh: true\n  description: >-\n    OAuth 2.0 Authorization Code flow. The user authorizes an application, selecting\n    which administrations to grant and which scopes (permissions) to allow. The\n    authorization code expires after 10 minutes; access tokens live 2 hours and are\n    renewed with a rotating refresh token that lasts 90 days from last use.\n  sources:\n  - https://docs.paytsoftware.com/authentication/authorization\n  - https://docs.paytsoftware.com/authentication/tokens\n- name: basic_client_credentials\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic (base64 client_id:client_secret, RFC 4648) is required only on the\n    token endpoints (/oauth/token) and the sign_up endpoint - used to obtain or\n    refresh tokens, not to call resource endpoints.\n  sources:\n\
  \  - https://docs.paytsoftware.com/authentication/basic-authorization\n- name: static_api_token\n  type: http\n  scheme: bearer\n  description: >-\n    Static API token fallback for clients unable to implement OAuth 2.0. Presented\n    as a Bearer token like an OAuth access token. Documented as the less-secure option.\n  sources:\n  - https://docs.paytsoftware.com/authentication/authorization\nmtls:\n  note: >-\n    Payt supports mutual TLS (mTLS) for webhook delivery: consumers may verify Payt's\n    client certificate (payt_mtls_certificate_2026.crt, valid until 2027-01-03),\n    downloadable from backend.paytsoftware.com. This is inbound webhook mTLS, not\n    required on outbound API calls.\n  source: https://docs.paytsoftware.com/webhooks/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payt/refs/heads/main/authentication/payt-authentication.yml
summary_line: oauth2/http · 4 schemes
tags:
- Company
- Applicative SaaS
- Accounts Receivable
- Order to Cash
- Invoicing
- Debt Collection
- Payments
- Fintech
- Credit Management
- Netherlands
---
