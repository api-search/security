---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: documented
name: Swapcard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swapcard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Swapcard
provider_slug: swapcard
scheme_count: 1
schemes:
- description: 'All Swapcard GraphQL queries require a valid access token passed in the Authorization header. Swapcard''s documented examples send the raw token value with no Bearer prefix (Authorization: ACCESS_TOKEN). Leads API tokens are created in the Exhibitor Center under Leads then API keys; Content (Event Admin) API access is provisioned to organizers. Tokens are secret - treat them like a password and never expose them in client-side code.'
  headerName: Authorization
  in: header
  name: accessToken
  sources:
  - https://swapcard.dev/exhibitors/authentication
  - https://swapcard.dev/leads-api/usage
  type: apiKey
slug: swapcard-authentication
source_filename: swapcard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://swapcard.dev/exhibitors/authentication\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  headerName: Authorization\n  description: 'All Swapcard GraphQL queries require a valid access token passed in\n    the Authorization header. Swapcard''s documented examples send the raw token\n    value with no Bearer prefix (Authorization: ACCESS_TOKEN). Leads API tokens are\n    created in the Exhibitor Center under Leads then API keys; Content (Event Admin)\n    API access is provisioned to organizers. Tokens are secret - treat them like a\n    password and never expose them in client-side code.'\n  sources:\n  - https://swapcard.dev/exhibitors/authentication\n  - https://swapcard.dev/leads-api/usage\nnotes: >-\n  Confirmed via live probe on 2026-07-12: an unauthenticated POST to\n  https://developer.swapcard.com/event-admin/graphql returns\n  {\"errors\":[{\"message\":\"You are\
  \ not authorized\",\"extensions\":{\"code\":\"UNAUTHORIZED\"}}]},\n  confirming token-gated access. The Content API and the Exhibitor Leads API use\n  separate endpoints and separate tokens.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swapcard/refs/heads/main/authentication/swapcard-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Events
- Event Management
- Community
- Networking
- Event Platform
- GraphQL
- Attendees
- Exhibitors
- SaaS
---
