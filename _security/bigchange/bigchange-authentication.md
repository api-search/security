---
api_key_in: []
api_specs:
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Jobs API
  slug: bigchange-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Contacts and Persons API
  slug: bigchange-contacts-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Finance API
  slug: bigchange-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Stock and Inventory API
  slug: bigchange-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Resources, Users and Vehicles API
  slug: bigchange-resources-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Notes and Worksheets API
  slug: bigchange-notes-worksheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Reference Data API
  slug: bigchange-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: swagger.json
  format: json
  label: BigChange Asset Management API
  slug: bigchange-asset-management-api
  spec_type: OpenAPI
  url: https://api.bigchange.com/swagger/asset-management/v1/swagger.json
- filename: swagger.json
  format: json
  label: BigChange Webhooks API
  slug: bigchange-webhooks-api
  spec_type: OpenAPI
  url: https://api.bigchange.com/swagger/webhooks/v1/swagger.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bigchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: BigChange secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BigChange
provider_slug: bigchange
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer JWT access token. Confirmed from BigChange''s published swagger security scheme (description: "Enter the access token only"). Sent as `Authorization: Bearer <access_token>`. Applies globally to the BigChange DX, Asset Management, and Webhooks APIs.'
  name: bearer
  scheme: bearer
  sources:
  - https://api.bigchange.com/swagger/v1/swagger.json
  - https://api.bigchange.com/swagger/asset-management/v1/swagger.json
  - https://api.bigchange.com/swagger/webhooks/v1/swagger.json
  type: http
slug: bigchange-authentication
source_filename: bigchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: https://api.bigchange.com/swagger/v1/swagger.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Bearer JWT access token. Confirmed from BigChange's published swagger security\n    scheme (description: \"Enter the access token only\"). Sent as\n    `Authorization: Bearer <access_token>`. Applies globally to the BigChange DX,\n    Asset Management, and Webhooks APIs.\n  sources:\n  - https://api.bigchange.com/swagger/v1/swagger.json\n  - https://api.bigchange.com/swagger/asset-management/v1/swagger.json\n  - https://api.bigchange.com/swagger/webhooks/v1/swagger.json\nrequiredHeaders:\n- name: Customer-Id\n  in: header\n  required: true\n  type: integer\n  format: int64\n  description: >-\n    The customer (BigChange account) identifier. Required on every operation in the\n    published spec, in addition to the Bearer token.\n  sources:\n  -\
  \ https://api.bigchange.com/swagger/v1/swagger.json\ntokenAcquisition:\n  reconciled: false\n  model: >-\n    Access tokens are obtained through BigChange's \"authentication proxy\" using an\n    API key issued in the developer portal under Account > Manage API Keys /\n    Integrations. The token is then presented as a Bearer JWT on API calls. The\n    exact token-exchange endpoint and grant type are documented on a\n    JavaScript-rendered portal page that did not scrape, so they are modeled here\n    rather than quoted. Live probes returned HTTP 401 (exists, auth required) for\n    https://api.bigchange.com/connect/token and https://api.bigchange.com/oauth/token,\n    and HTTP 404 for https://api.bigchange.com/auth/v1/token - the canonical token\n    URL is not asserted.\n  sources:\n  - https://developers.bigchange.com/docs/rest/auth-proxy/get-an-access-token\n  - https://developers.bigchange.com/account/integrations\nlegacyApi:\n  note: >-\n    A separate legacy JobWatch web-services\
  \ API (host webservice.bigchange.com) is\n    authenticated with an API key plus the BigChange account username and password\n    (per the Cyclr JobWatch connector guide). This is distinct from the modern\n    Bearer-JWT REST API above.\n  sources:\n  - https://community.cyclr.com/connector-guides/bigchange-jobwatch/bigchange-jobwatch-setup\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/authentication/bigchange-authentication.yml
summary_line: http · 1 scheme
tags:
- Field Service Management
- Job Management
- Scheduling
- Workforce Management
- Fleet
- CRM
- SaaS
---
