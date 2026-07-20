---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Eversports Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eversports secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eversports
provider_slug: eversports
scheme_count: 1
schemes:
- applies_to:
  - graphql/eversports-provider-api.graphql
  - graphql/eversports-aggregator.graphql
  header: 'Authorization: Bearer <TOKEN>'
  name: bearerAuth
  provisioning: Contact support@eversports.com; Eversports issues access credentials plus a Quick Start Guide.
  scheme: bearer
  sources:
  - graphql/eversports-provider-api-introspection.json
  - graphql/eversports-aggregator-introspection.json
  type: http
slug: eversports-authentication
source_filename: eversports-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://helpcenter.eversportsmanager.com/what-is-the-provider-api\ndocs: https://helpcenter.eversportsmanager.com/what-is-the-provider-api\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Both Eversports GraphQL APIs authenticate with a static Bearer token issued\n    by Eversports on request. There is no self-serve OAuth flow and no documented\n    scope surface; the opaque token is scoped to the provider/venue account that\n    Eversports provisions. Tokens are sent on every HTTP request.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer <TOKEN>'\n    provisioning: Contact support@eversports.com; Eversports issues access credentials plus a Quick Start Guide.\n    applies_to:\n      - graphql/eversports-provider-api.graphql\n      - graphql/eversports-aggregator.graphql\n    sources:\n      - graphql/eversports-provider-api-introspection.json\n\
  \      - graphql/eversports-aggregator-introspection.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eversports/refs/heads/main/authentication/eversports-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Sports
- Fitness
- Booking
- Scheduling
- Wellness
- GraphQL
- Reservations
- Events
---
