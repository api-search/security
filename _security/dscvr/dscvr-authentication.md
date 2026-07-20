---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Dscvr Authentication
name_suffix: Authentication
oauth_flows: []
overview: DSCVR secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DSCVR
provider_slug: dscvr
scheme_count: 1
schemes:
- applied_to: https://api.dscvr.one/graphql
  description: Unauthenticated public GraphQL endpoint; logged-out-user permission scope.
  name: public
  type: none
slug: dscvr-authentication
source_filename: dscvr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.dscvr.one/build/dscvr-api/\ndocs: https://docs.dscvr.one/build/dscvr-api/\nsummary:\n  types: [none]\n  note: >-\n    The DSCVR GraphQL API currently requires no authentication. Per the docs, \"queries are made\n    with the permissions of a logged out user.\" The docs note that authentication and rate-limiting\n    may be introduced in the future to scale the API. There are no API keys, OAuth flows, or bearer\n    tokens at this time.\nschemes:\n- name: public\n  type: none\n  applied_to: https://api.dscvr.one/graphql\n  description: Unauthenticated public GraphQL endpoint; logged-out-user permission scope.\ncanvas_note: >-\n  The DSCVR Canvas framework performs a postMessage handshake between an embedded iframe app and\n  the DSCVR host (via @dscvr-one/canvas-client-sdk); the host supplies the current user/content\n  context. This is a host-mediated trust model, not an API credential exchanged by the developer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dscvr/refs/heads/main/authentication/dscvr-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Social
- Web3
- GraphQL
- Blockchain
- Solana
- Internet Computer
- SocialFi
- Social Graph
- Developer Platform
---
