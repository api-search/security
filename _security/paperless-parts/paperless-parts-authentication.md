---
api_key_in:
- header
api_specs:
- filename: paperless-parts-contacts-api-openapi.yml
  format: yaml
  label: Paperless Parts Contacts API
  slug: paperless-parts-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-contacts-api-openapi.yml
- filename: paperless-parts-custom-tables-api-openapi.yml
  format: yaml
  label: Paperless Parts Custom Tables API
  slug: paperless-parts-custom-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-custom-tables-api-openapi.yml
- filename: paperless-parts-customers-api-openapi.yml
  format: yaml
  label: Paperless Parts Customers API
  slug: paperless-parts-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-customers-api-openapi.yml
- filename: paperless-parts-events-api-openapi.yml
  format: yaml
  label: Paperless Parts Events API
  slug: paperless-parts-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-events-api-openapi.yml
- filename: paperless-parts-integration-actions-api-openapi.yml
  format: yaml
  label: Paperless Parts Integration Actions API
  slug: paperless-parts-integration-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-integration-actions-api-openapi.yml
- filename: paperless-parts-jobs-api-openapi.yml
  format: yaml
  label: Paperless Parts Jobs API
  slug: paperless-parts-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-jobs-api-openapi.yml
- filename: paperless-parts-orders-api-openapi.yml
  format: yaml
  label: Paperless Parts Orders API
  slug: paperless-parts-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-orders-api-openapi.yml
- filename: paperless-parts-parts-api-openapi.yml
  format: yaml
  label: Paperless Parts Parts API
  slug: paperless-parts-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-parts-api-openapi.yml
- filename: paperless-parts-processes-api-openapi.yml
  format: yaml
  label: Paperless Parts Processes API
  slug: paperless-parts-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-processes-api-openapi.yml
- filename: paperless-parts-purchased-components-api-openapi.yml
  format: yaml
  label: Paperless Parts Purchased Components API
  slug: paperless-parts-purchased-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-purchased-components-api-openapi.yml
- filename: paperless-parts-quote-items-api-openapi.yml
  format: yaml
  label: Paperless Parts Quote Items API
  slug: paperless-parts-quote-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-quote-items-api-openapi.yml
- filename: paperless-parts-quotes-api-openapi.yml
  format: yaml
  label: Paperless Parts Quotes API
  slug: paperless-parts-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/openapi/paperless-parts-quotes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Paperless Parts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paperless Parts secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paperless Parts
provider_slug: paperless-parts
scheme_count: 1
schemes:
- applies_to: every operation in both v1 and v2 (declared as a document-level security requirement)
  description: API key to authorize requests.
  in: header
  name: app_id
  parameter: Authorization
  sources:
  - openapi/paperless-parts-v1-openapi.yml
  - openapi/paperless-parts-v2-openapi.yml
  type: apiKey
  value_format: API-Token <api_token>
slug: paperless-parts-authentication
source_filename: paperless-parts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  openapi/paperless-parts-v1-openapi.yml , openapi/paperless-parts-v2-openapi.yml ,\n  https://www.paperlessparts.com/api/ , https://github.com/part-os/core-python\ndocs: https://www.paperlessparts.com/api/\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\nmodel: >-\n  A single account-scoped API token, sent in the Authorization header with an \"API-Token \" prefix.\n  There is no OAuth 2.0, no OpenID Connect, no mTLS and no scope system — the token that reads a\n  quote is the same token that can facilitate an order or bulk-overwrite a pricing table. An agent\n  cannot be granted a narrower credential.\nschemes:\n  - name: app_id\n    type: apiKey\n    in: header\n    parameter: Authorization\n    value_format: 'API-Token <api_token>'\n    description: API key to authorize requests.\n    applies_to: every operation in both v1\
  \ and v2 (declared as a document-level security requirement)\n    sources:\n      - openapi/paperless-parts-v1-openapi.yml\n      - openapi/paperless-parts-v2-openapi.yml\nissuance:\n  location: Paperless Parts application, Settings > Integrations > API Token\n  actor: account administrator\n  self_serve: false\n  requires: an active Paperless Parts subscription — there is no public developer signup\nlifecycle:\n  create: true\n  revoke: true\n  regenerate: true\n  rotation_policy: not published\n  expiry: not published\n  source: https://www.paperlessparts.com/api/\nscoping:\n  granularity: account-wide\n  scopes: none\n  per_environment_keys: not published\n  test_vs_live_prefix: none published\n  note: >-\n    The token has no visible prefix convention (unlike sk_test_/sk_live_ style schemes), so an\n    integration cannot tell from the credential alone which account or environment it addresses.\nsdk_handling:\n  repository: https://github.com/part-os/core-python\n  note: >-\n    \"\
  The SDK handles this for you when you include this access token when instantiating your\n    PaperlessClient object\" — the SDK README also warns that the token \"should never be committed\n    to your version control system\".\ngaps:\n  - no OAuth 2.0 or OIDC, so no delegated or user-consented access\n  - no scopes, so no least-privilege credential for an agent or a partner\n  - no documented token expiry or rotation policy\n  - no separate sandbox/test credential documented\n  - no 401 or 403 response declared on any operation in either published OpenAPI\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperless-parts/refs/heads/main/authentication/paperless-parts-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Manufacturing
- Quoting
- CNC Machining
- Sheet Metal
- ERP
- CRM
- Job Shops
- Aerospace and Defense
- Pricing
- Estimating
- Industrial
---
