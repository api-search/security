---
api_key_in:
- header
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: searched
name: Voyceme Authentication
name_suffix: Authentication
oauth_flows: []
overview: VoyceMe secures its APIs with none and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VoyceMe
provider_slug: voyceme
scheme_count: 3
schemes:
- description: Hasura anonymous role; public read + public form-insert mutations, no credential.
  name: anonymous
  sources:
  - graphql/voyceme-graphql.graphql
  type: none
- description: Hasura admin secret for privileged access (not publicly provisioned).
  in: header
  name: HasuraAdminSecret
  parameter_name: x-hasura-admin-secret
  sources:
  - graphql/voyceme-graphql.graphql
  type: apiKey
- description: Bearer API token for Play Engine REST endpoints (api/character-create, playengine/chat).
  name: PlayEngineBearer
  scheme: bearer
  sources:
  - https://playengine.voyce.me/developers/
  type: http
slug: voyceme-authentication
source_filename: voyceme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: live probe of https://graphql.voyce.me/v1/graphql + https://playengine.voyce.me/developers/\nsummary:\n  types: [none, http]\n  api_key_in: [header]\n  oauth2_flows: []\nnotes: >-\n  VoyceMe exposes a public Hasura GraphQL endpoint at https://graphql.voyce.me/v1/graphql.\n  Read queries and the public insert mutations (contact_us, newsletter, popup_emails,\n  search_history, giveaway participants, CSAT, chatbot conversations/messages, feedback,\n  user_creations) execute against Hasura's anonymous role and require NO authentication\n  (verified: an unauthenticated query returned live voyce_series and blog_posts data).\n  Privileged/admin access to the same Hasura instance uses the standard Hasura auth model\n  (x-hasura-admin-secret header or a JWT bearer carrying x-hasura-* session claims) but no\n  admin surface is publicly documented. The Play Engine developer product\n  (https://playengine.voyce.me/developers/) uses a bearer\
  \ API token (a \"demo\" token is\n  referenced in the public app config) for its REST character/chat endpoints.\nschemes:\n  - name: anonymous\n    type: none\n    description: Hasura anonymous role; public read + public form-insert mutations, no credential.\n    sources: [graphql/voyceme-graphql.graphql]\n  - name: HasuraAdminSecret\n    type: apiKey\n    in: header\n    parameter_name: x-hasura-admin-secret\n    description: Hasura admin secret for privileged access (not publicly provisioned).\n    sources: [graphql/voyceme-graphql.graphql]\n  - name: PlayEngineBearer\n    type: http\n    scheme: bearer\n    description: Bearer API token for Play Engine REST endpoints (api/character-create, playengine/chat).\n    sources: [https://playengine.voyce.me/developers/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyceme/refs/heads/main/authentication/voyceme-authentication.yml
summary_line: none/http · 3 schemes
tags:
- Company
- Manga
- Webtoons
- Web Novels
- Comics
- Publishing
- Creators
- GraphQL
- AI Characters
- Entertainment
- Media
---
