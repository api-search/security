---
api_key_in:
- header
api_specs:
- filename: choozle-accounts-api-openapi.yml
  format: yaml
  label: Choozle Accounts API
  slug: choozle-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choozle/refs/heads/main/openapi/choozle-accounts-api-openapi.yml
- filename: choozle-authorization-api-openapi.yml
  format: yaml
  label: Choozle Authorization API
  slug: choozle-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choozle/refs/heads/main/openapi/choozle-authorization-api-openapi.yml
- filename: choozle-reports-api-openapi.yml
  format: yaml
  label: Choozle Reports API
  slug: choozle-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choozle/refs/heads/main/openapi/choozle-reports-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Choozle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Choozle secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Choozle
provider_slug: choozle
scheme_count: 1
schemes:
- applies_to:
  - listAccounts
  - getReports
  description: 'Authentication token generated from the /api/auth endpoint. Valid for two hours from creation. Sent as the `token` request header — not Authorization: Bearer.'
  in: header
  name: tokenHeader
  parameter: token
  sources:
  - openapi/_original/openapi.yml
  - openapi/choozle-accounts-api-openapi.yml
  - openapi/choozle-reports-api-openapi.yml
  type: apiKey
slug: choozle-authentication
source_filename: choozle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.choozle.com/connecting-to-choozles-reporting-api\ndocs:\n  - https://help.choozle.com/connecting-to-choozles-reporting-api\n  - https://app.choozle.com/apidoc/\nalso_derived_from:\n  - openapi/_original/openapi.yml\n  - https://app.choozle.com/apidoc/api_data.json\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  model: signed-handshake-then-opaque-token\n  note: >-\n    Not a static API key despite the apiKey scheme type. Choozle uses a two-step\n    model: an HMAC-SHA256 signed request exchanges a long-lived private key for\n    a short-lived opaque token, and only that token is sent on subsequent calls.\n    The private key itself never travels on a reporting request.\nschemes:\n  - name: tokenHeader\n    type: apiKey\n    in: header\n    parameter: token\n    description: >-\n      Authentication token generated from the /api/auth endpoint. Valid for two\n      hours from\
  \ creation. Sent as the `token` request header — not\n      Authorization: Bearer.\n    sources:\n      - openapi/_original/openapi.yml\n      - openapi/choozle-accounts-api-openapi.yml\n      - openapi/choozle-reports-api-openapi.yml\n    applies_to:\n      - listAccounts\n      - getReports\nhandshake:\n  endpoint: POST https://app.choozle.com/api/auth\n  unauthenticated: true\n  content_type: application/x-www-form-urlencoded\n  parameter_location: body\n  parameter_location_note: >-\n    Parameters must be in the BODY, not the header. The provider lists sending\n    them as headers as a common troubleshooting failure.\n  parameters:\n    - name: email\n      required: true\n      type: string\n      description: >-\n        The email on the API profile. Google-hosted mailboxes can use a plus\n        alias (user+api@choozle.com) so the API identity is a distinct address\n        that still delivers to the human's inbox.\n    - name: timestamp\n      required: true\n      type: ISO\
  \ 8601 datetime\n      example: '2015-05-04T11:34:02-06:00'\n      constraint: must be within five minutes of the Choozle server's current time\n    - name: signature\n      required: true\n      type: string\n      description: >-\n        HMAC-SHA256 digest of the concatenation of the submitted email and\n        timestamp, keyed with the API private key.\n      encoding: lowercase hex\n      encoding_constraint: >-\n        Lowercase hex only. Uppercase hex and base64 are both rejected, and this\n        is the provider's first-listed troubleshooting issue.\n  returns:\n    field: token\n    type: string\n    ttl_seconds: 7200\n    refresh: none — re-run the handshake\ncredentials:\n  self_service: false\n  issuance: >-\n    An ORG admin or advertiser admin creates an API profile/username for the\n    account, at which point the system generates an API secret key. The key is\n    released only by submitting a ticket through the Choozle Customer Portal.\n    There is no self-service\
  \ key page and no key-management API.\n  rotation: not documented\n  scopes: none\n  scopes_note: >-\n    There is no scope or permission model on the API. Access is all-or-nothing\n    at the account level, determined by which accounts the API profile is\n    attached to.\n  api_only_role: >-\n    \"API Only access: Full access to account data through the API, including\n    campaign and ad group reporting data. An API Only user cannot view, edit, or\n    otherwise access the account from the website.\" This is a genuine least-\n    privilege control — a machine credential that cannot log into the UI.\ntransport:\n  https_only: true\n  tls_version: TLSv1.3\n  hsts: false\n  hsts_note: >-\n    app.choozle.com does not send Strict-Transport-Security, so the credential\n    exchange is not HSTS-protected even though it is HTTPS-only in practice.\nfailure_modes:\n  - status: 401\n    body: '{\"error\": \"Request incomplete\"}'\n    cause: missing or unverifiable email/timestamp/signature\
  \ on the handshake\n  - status: 401\n    body: '{\"error\": \"Unauthorized - No Token Found in request\"}'\n    cause: no `token` header on a reporting call\n  - status: 401\n    body: '{\"error\": \"Unauthorized - Token is expired\"}'\n    cause: token older than two hours\nsee: errors/choozle-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/choozle/refs/heads/main/authentication/choozle-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Digital Advertising
- Programmatic Advertising
- DSP
- Demand-Side Platform
- Advertising Reporting
- Campaign Reporting
- Display Advertising
- Connected TV
- CTV
- Video Advertising
- Native Advertising
- DOOH
- Reporting
- Real-Time Bidding
- RTB
- AdTech
---
