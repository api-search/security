---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gigs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gigs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gigs
provider_slug: gigs
scheme_count: 1
schemes:
- description: Gigs authenticates every request with a project-scoped API key sent as a Bearer token. An organization can hold multiple projects (e.g. production, test, experiment), and each project issues one or more unique API keys managed in the developers section of the Gigs Dashboard. A key grants full access to all data in its project; rotation and expiry dates are recommended.
  format: 'Authorization: Bearer ${GIGS_TOKEN}'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developers.gigs.com/api/authentication
  type: http
slug: gigs-authentication
source_filename: gigs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.gigs.com/api/authentication\ndocs: https://developers.gigs.com/api/authentication\nsummary:\n  types:\n  - http\n  http_scheme: bearer\n  token_location: header\n  header: Authorization\n  key_management: per-project API keys\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer ${GIGS_TOKEN}'\n  description: 'Gigs authenticates every request with a project-scoped API key sent\n    as a Bearer token. An organization can hold multiple projects (e.g. production,\n    test, experiment), and each project issues one or more unique API keys managed\n    in the developers section of the Gigs Dashboard. A key grants full access to all\n    data in its project; rotation and expiry dates are recommended.'\n  sources:\n  - https://developers.gigs.com/api/authentication\nerrors:\n  unauthenticated:\n    status: 401\n    type: unauthenticated\n\
  \    message: Invalid authorization token\nnotes: No OAuth2/OIDC surface is documented; api.gigs.com returns 401 to all unauthenticated\n  requests. Keys are managed at https://dashboard.gigs.com/developers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigs/refs/heads/main/authentication/gigs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Telecom
- Connectivity
- eSIM
- MVNO
- Mobile
- Subscriptions
- Payments
- Webhooks
- Embedded Finance
---
