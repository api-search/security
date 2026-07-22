---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Metamarkets Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metamarkets secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metamarkets
provider_slug: metamarkets
scheme_count: 1
schemes:
- credential_source: username + password issued by a Metamarkets data engineer / account representative (per-endpoint)
  header: Authorization
  in: header
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.metamarkets.com/docs/real-time-data-delivery
  - https://docs.metamarkets.com/docs/rdi-client-library
  transport: https-required
  type: http
slug: metamarkets-authentication
source_filename: metamarkets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.metamarkets.com/docs/real-time-data-delivery\nnote: >-\n  The Metamarkets RDI ingestion endpoints are protected by HTTP Basic\n  authentication. Each customer receives a username, password, and one or more\n  endpoint URLs from their Metamarkets data engineer / account representative;\n  credentials are not self-service. HTTPS is required so credentials are sent\n  encrypted. Documented via the RDI client library and the real-time delivery\n  curl example (`--user <username>:<password>`).\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  self_service: false\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    in: header\n    header: Authorization\n    transport: https-required\n    credential_source: >-\n      username + password issued by a Metamarkets data engineer / account\n      representative (per-endpoint)\n    sources:\n      - https://docs.metamarkets.com/docs/real-time-data-delivery\n\
  \      - https://docs.metamarkets.com/docs/rdi-client-library\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metamarkets/refs/heads/main/authentication/metamarkets-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Advertising
- AdTech
- Analytics
- Real Time
- Data Ingestion
- Programmatic Advertising
- OpenRTB
- Business Intelligence
---
