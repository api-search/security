---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mlsgrid-lookup-api-openapi.yml
  format: yaml
  label: mlsgrid Lookup API
  slug: mlsgrid-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-lookup-api-openapi.yml
- filename: mlsgrid-media-api-openapi.yml
  format: yaml
  label: mlsgrid Media API
  slug: mlsgrid-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-media-api-openapi.yml
- filename: mlsgrid-member-api-openapi.yml
  format: yaml
  label: mlsgrid Member API
  slug: mlsgrid-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-member-api-openapi.yml
- filename: mlsgrid-metadata-api-openapi.yml
  format: yaml
  label: mlsgrid Metadata API
  slug: mlsgrid-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-metadata-api-openapi.yml
- filename: mlsgrid-office-api-openapi.yml
  format: yaml
  label: mlsgrid Office API
  slug: mlsgrid-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-office-api-openapi.yml
- filename: mlsgrid-openhouse-api-openapi.yml
  format: yaml
  label: mlsgrid OpenHouse API
  slug: mlsgrid-openhouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-openhouse-api-openapi.yml
- filename: mlsgrid-property-api-openapi.yml
  format: yaml
  label: mlsgrid Property API
  slug: mlsgrid-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-property-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mlsgrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mlsgrid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mlsgrid
provider_slug: mlsgrid
scheme_count: 1
schemes:
- bearerFormat: OAuth2
  description: Long-lived OAuth 2.0 bearer token issued via the MLS Grid web application token tab.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mlsgrid-lookup-api-openapi.yml
  - openapi/mlsgrid-media-api-openapi.yml
  - openapi/mlsgrid-member-api-openapi.yml
  - openapi/mlsgrid-metadata-api-openapi.yml
  - openapi/mlsgrid-office-api-openapi.yml
  - openapi/mlsgrid-openhouse-api-openapi.yml
  - openapi/mlsgrid-property-api-openapi.yml
  type: http
slug: mlsgrid-authentication
source_filename: mlsgrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\ndocs:\n- https://docs.mlsgrid.com/master.md\n- https://docs.mlsgrid.com/api-documentation/api-version-2.0.md\n- https://docs.mlsgrid.com/data-consumer-guides/how-to-register-and-activate-an-mls-grid-data-consumer-account.md\nsource: https://docs.mlsgrid.com/master.md + openapi/mlsgrid-lookup-api-openapi.yml, openapi/mlsgrid-media-api-openapi.yml, openapi/mlsgrid-member-api-openapi.yml,\n  openapi/mlsgrid-metadata-api-openapi.yml, openapi/mlsgrid-office-api-openapi.yml, openapi/mlsgrid-openhouse-api-openapi.yml,\n  openapi/mlsgrid-property-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  description: Long-lived OAuth 2.0 bearer token issued via the MLS Grid web application token\n    tab.\n  sources:\n  - openapi/mlsgrid-lookup-api-openapi.yml\n  - openapi/mlsgrid-media-api-openapi.yml\n  - openapi/mlsgrid-member-api-openapi.yml\n  - openapi/mlsgrid-metadata-api-openapi.yml\n\
  \  - openapi/mlsgrid-office-api-openapi.yml\n  - openapi/mlsgrid-openhouse-api-openapi.yml\n  - openapi/mlsgrid-property-api-openapi.yml\nmodel:\n  flavor: simplified-oauth2-bearer\n  header: 'Authorization: Bearer <access_token>'\n  token_lifetime: long-lived\n  token_endpoint: null\n  authorization_endpoint: null\n  refresh_flow: false\n  scopes: false\n  scopes_note: >-\n    No scope surface exists, so no scopes/ artifact is written. Entitlement is not expressed in the\n    token - it arrives in the payload, per record, as MlgCanUse (IDX | VOW | BO | PT) and MlgCanView.\n  discovery:\n    openid_configuration: false\n    oauth_authorization_server: false\n    note: >-\n      Probed 2026-09-17 across www / api / docs / app.mlsgrid.com. 404 on www and docs, 401 on\n      api.mlsgrid.com (which authenticates every path including /.well-known/*), and the app host\n      answers 200 with its SPA shell. See well-known/mlsgrid-well-known.yml.\n  issuance:\n    self_serve: false\n    steps:\n\
  \    - Submit the interest form at https://www.mlsgrid.com/interest-form\n    - Sign the MLS Grid Master Data License Agreement in the licensing portal\n    - Create a data subscription and add a licensee\n    - Wait for the originating MLS to approve the licensee\n    - Read the long-lived token from the token tab of the approved subscription in app.mlsgrid.com\n    source: https://docs.mlsgrid.com/data-consumer-guides/how-to-register-and-activate-an-mls-grid-data-consumer-account.md\n  rotation: >-\n    Contact support@mlsgrid.com to have a token re-generated, which invalidates the old one. No\n    self-service rotation endpoint is published.\n  suspension: >-\n    Exceeding a published rate limit suspends the access token and emails the vendor account primary\n    contact; it is reinstated automatically once usage falls back within limits.\n  gotcha: >-\n    Compression is evaluated BEFORE authentication. A request without Accept-Encoding gzip returns\n    HTTP 400 COMPRESSION REQUIRED,\
  \ not 401 - which reads as an auth failure to a client that only\n    checks for 401.\n  media_credential_reuse: >-\n    Media downloads must send a User-Agent header whose value is the OAuth 2 access token (enforced\n    from 2026-06-01), so the credential is carried in two different headers depending on the surface.\nreverified_on: '2026-09-17'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/authentication/mlsgrid-authentication.yml
summary_line: http · 1 scheme
tags:
- Real-Estate
- Property Listings
- MLS
- RESO
- Data Replication
- OData
- Housing
- Data Licensing
- IDX
- Property Data
---
