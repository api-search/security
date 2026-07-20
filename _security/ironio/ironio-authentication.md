---
api_key_in:
- header
- query
auth_types:
- oauth2-token
description: ''
kind: authentication
layout: security
method: searched
name: Ironio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iron.io secures its APIs with oauth2-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Iron.io
provider_slug: ironio
scheme_count: 2
schemes:
- description: 'Bearer-style token passed in the Authorization header using the "OAuth" scheme: `Authorization: OAuth <TOKEN>`. Tokens are obtained from the HUD and are shared across IronMQ, IronWorker, and IronCache.'
  header_format: 'Authorization: OAuth <TOKEN>'
  in: header
  name: OAuthToken
  scheme: bearer
  sources:
  - docs
  type: http
- description: 'The same token may alternatively be supplied as an `oauth` query-string parameter (documented for IronWorker): `?oauth=<TOKEN>`.'
  in: query
  name: OAuthTokenQuery
  parameter: oauth
  sources:
  - docs
  type: apiKey
slug: ironio-authentication
source_filename: ironio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://dev.iron.io/worker/reference/api/\ndocs: https://dev.iron.io/worker/reference/api/\nsummary:\n  types: [oauth2-token]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  notes: >-\n    Iron.io uses a static per-project OAuth token (not a full OAuth2 authorization\n    flow). The token is issued from the Iron.io HUD and works across all Iron.io\n    services (IronMQ, IronWorker, IronCache). Every request also carries a Project ID\n    in the URL path.\nschemes:\n- name: OAuthToken\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer-style token passed in the Authorization header using the \"OAuth\" scheme:\n    `Authorization: OAuth <TOKEN>`. Tokens are obtained from the HUD and are shared\n    across IronMQ, IronWorker, and IronCache.\n  in: header\n  header_format: 'Authorization: OAuth <TOKEN>'\n  sources: [docs]\n- name: OAuthTokenQuery\n  type: apiKey\n  in: query\n  parameter: oauth\n  description:\
  \ >-\n    The same token may alternatively be supplied as an `oauth` query-string\n    parameter (documented for IronWorker): `?oauth=<TOKEN>`.\n  sources: [docs]\nproject_scoping:\n  required: true\n  location: url-path\n  pattern: /{version}/projects/{Project ID}/...\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironio/refs/heads/main/authentication/ironio-authentication.yml
summary_line: oauth2-token · 2 schemes
tags:
- Company
- Infrastructure
- Message Queue
- Serverless
- Background Jobs
- Task Processing
- Cache
- Messaging
---
