---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fis-accounts-api-openapi.yml
  format: yaml
  label: FIS Global Accounts API
  slug: fis-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-accounts-api-openapi.yml
- filename: fis-ach-api-openapi.yml
  format: yaml
  label: FIS Global ACH API
  slug: fis-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-ach-api-openapi.yml
- filename: fis-payments-api-openapi.yml
  format: yaml
  label: FIS Global Payments API
  slug: fis-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-payments-api-openapi.yml
- filename: fis-transactions-api-openapi.yml
  format: yaml
  label: FIS Global Transactions API
  slug: fis-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-transactions-api-openapi.yml
- filename: fis-wire-transfers-api-openapi.yml
  format: yaml
  label: FIS Global Wire Transfers API
  slug: fis-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-wire-transfers-api-openapi.yml
- filename: fis-accounting-data-as-a-service-openapi.json
  format: json
  label: FIS Accounting Data as a Service
  slug: fis-accounting-data-as-a-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/_original/fis-accounting-data-as-a-service-openapi.json
auth_types:
- http
- basic
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fis Authentication
name_suffix: Authentication
oauth_flows: []
overview: FIS Global secures its APIs with http and basic across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FIS Global
provider_slug: fis
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/_original/fis-accounting-data-as-a-service-openapi.json
  - https://docs.railz.ai/reference/authentication
  type: http
- name: basic
  scheme: basic
  sources:
  - https://docs.railz.ai/reference/authentication
  type: http
  used_for: token minting only
slug: fis-authentication
source_filename: fis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: https://docs.railz.ai/reference/authentication\ndocs: https://docs.railz.ai/reference/authentication\nsupersedes:\n  note: >-\n    Replaces the 2026-07-11 derived profile, which read its OAuth2 clientCredentials scheme and\n    a tokenUrl of https://api.fisglobal.com/oauth/token out of openapi/_original/fis-payments-openapi.yml.\n    That host does not resolve in DNS and the scheme is not corroborated by any FIS document\n    that can be reached without a Code Connect account, so it is not carried forward as fact.\nsummary:\n  types:\n  - http\n  - basic\n  oauth2_flows: []\n  note: >-\n    Two distinct authentication surfaces, only one of which is publicly documented.\nsurfaces:\n- api: FIS Accounting Data as a Service\n  base_url: https://api.railz.ai\n  documented: true\n  model: two-step bearer\n  steps:\n  - step: 1\n    name: Mint an access token\n    description: >-\n      HTTP Basic against the Get Access Token endpoint.\
  \ The API identifier client_id is the\n      Basic username and the secret_key is the password, base64 encoded.\n    scheme: basic\n  - step: 2\n    name: Call the API\n    description: 'Present the minted token as an Authorization header: Bearer <access_token>, on every request.'\n    scheme: bearer\n  token:\n    lifetime_minutes: 60\n    format: JWT\n    guidance: The docs recommend minting a fresh access_token before each call rather than caching to the edge of its life.\n  credentials:\n    key_prefixes:\n      sandbox: SB_\n      production: ID_\n    max_keys_per_team: 5\n    rotation: Keys never expire on their own; revocation is by deleting the key in the Dashboard.\n  transport:\n    https_required: true\n    note: 'Docs state plainly: calls made over plain HTTP will fail.'\n  spec_evidence:\n    file: openapi/_original/fis-accounting-data-as-a-service-openapi.json\n    securitySchemes:\n    - name: bearer\n      type: http\n      scheme: bearer\n      bearerFormat: JWT\n    applied:\
  \ false\n    gap: >-\n      The contract DEFINES the bearer scheme in components.securitySchemes but declares no\n      top-level `security` and applies it to none of the 233 operations. A generated client\n      reading the spec alone would send no credential and take a 401 on every call; the\n      requirement is only in prose.\n- api: FIS Code Connect (core banking, payments, wealth)\n  base_url: null\n  documented: false\n  model: unknown\n  note: >-\n    Code Connect documents authentication at\n    https://codeconnect.fisglobal.com/app/guides/authenticate, but that route renders inside an\n    Angular application that serves the same shell to an unauthenticated crawler, and the\n    marketplace requires a reviewed registration before the catalog or the key-generation flow\n    is visible. The auth model is therefore not publicly readable, and none is asserted here.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/_original/fis-accounting-data-as-a-service-openapi.json\n\
  \  - https://docs.railz.ai/reference/authentication\n- name: basic\n  type: http\n  scheme: basic\n  used_for: token minting only\n  sources:\n  - https://docs.railz.ai/reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/authentication/fis-authentication.yml
summary_line: http/basic · 2 schemes
tags:
- Banking
- Core Banking
- Financial-Services
- Payments
- Fintech
---
