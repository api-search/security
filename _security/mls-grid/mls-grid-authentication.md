---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mls Grid Authentication
name_suffix: Authentication
oauth_flows: []
overview: MLS Grid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MLS Grid
provider_slug: mls-grid
scheme_count: 1
schemes:
- bearerFormat: OAuth 2.0 access token (long-lived)
  description: MLS Grid describes its scheme as "a simplified Oauth 2 authentication schema with long term tokens" — there is no token endpoint and no authorization-code round trip. Trust is established out of band through the subscription sign-up process; the token is generated inside the MLS Grid web application and pasted into the Authorization header.
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.mlsgrid.com/master.md
  - https://docs.mlsgrid.com/api-documentation/api-version-2.0.md
  type: http
  value_template: Bearer <access_token>
slug: mls-grid-authentication
source_filename: mls-grid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://docs.mlsgrid.com/master.md\ndocs: https://docs.mlsgrid.com/master.md#authentication\nnote: >-\n  No OpenAPI or OData $metadata document could be retrieved anonymously (every anonymous call to\n  api.mlsgrid.com returns HTTP 401), so this profile is read from the public documentation rather\n  than derived from a machine-readable contract.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  self_serve: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth 2.0 access token (long-lived)\n  in: header\n  header: Authorization\n  value_template: 'Bearer <access_token>'\n  description: >-\n    MLS Grid describes its scheme as \"a simplified Oauth 2 authentication schema with long term\n    tokens\" — there is no token endpoint and no authorization-code round trip. Trust is established\n    out of band through the subscription sign-up process; the token is generated inside\
  \ the MLS Grid\n    web application and pasted into the Authorization header.\n  sources:\n  - https://docs.mlsgrid.com/master.md\n  - https://docs.mlsgrid.com/api-documentation/api-version-2.0.md\nissuance:\n  self_serve: false\n  flow: >-\n    1) Accept the MLS Grid Master Data License Agreement through the MLS Grid online licensing\n    portal. 2) Have a data subscription created and a licensee added. 3) Be approved by the\n    originating MLS. Only then is an API token generated and presented on the token tab when viewing\n    a subscription in the MLS Grid web application.\n  console: https://app.mlsgrid.com/\n  license_agreement: https://www.mlsgrid.com/s/MLS-GRID-Data-License-Agreement.pdf\n  rotation: >-\n    Contact support@mlsgrid.com to have the token re-generated; regeneration invalidates the old\n    token. No self-service rotation endpoint is documented.\n  expiry: Long-lived; no documented TTL or refresh flow.\nadditional_requirements:\n- requirement: gzip\n  detail: >-\n\
  \    Every request must send an Accept-Encoding header containing gzip. Without it the service\n    returns HTTP 400 \"COMPRESSION REQUIRED\" before it evaluates authentication.\n  source: https://docs.mlsgrid.com/api-documentation/api-version-2.0.md\n- requirement: media-user-agent\n  detail: >-\n    Requests that download media from a MediaURL must send an HTTP User-Agent header whose value is\n    the OAuth 2 access token itself. From 2026-06-01 any other User-Agent is denied media access.\n  source: https://docs.mlsgrid.com/releases/changes-to-mls-grid-media-access.md\nscopes:\n  documented: false\n  note: >-\n    No OAuth scope surface is published. Authorization is expressed per record in the payload\n    (MlgCanUse use-case array and the MlgCanView license flag) and per subscription (feed type:\n    IDX / VOW / BO / PT), not as token scopes.\ndiscovery:\n  probed:\n  - url: https://api.mlsgrid.com/.well-known/openid-configuration\n    status: 401\n  - url: https://app.mlsgrid.com/.well-known/openid-configuration\n\
  \    status: 200\n    note: Returns the web application's HTML SPA shell, not an OIDC discovery document.\n  - url: https://app.mlsgrid.com/.well-known/oauth-authorization-server\n    status: 200\n    note: Returns the web application's HTML SPA shell, not an RFC 8414 metadata document.\n  - url: https://www.mlsgrid.com/.well-known/openid-configuration\n    status: 404\n  openid_connect: false\n  rfc8414: false\n  probed_on: '2026-07-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mls-grid/refs/heads/main/authentication/mls-grid-authentication.yml
summary_line: http · 1 scheme
tags:
- Real-Estate
- United States
- MLS
- RESO
- Property Listings
- IDX
- PropTech
- OData
- Data Licensing
---
