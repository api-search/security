---
api_key_in: []
api_specs:
- filename: liveblocks-active-users-api-openapi.yml
  format: yaml
  label: Liveblocks Active Users API
  slug: liveblocks-active-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/openapi/liveblocks-active-users-api-openapi.yml
- filename: liveblocks-comments-api-openapi.yml
  format: yaml
  label: Liveblocks Comments API
  slug: liveblocks-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/openapi/liveblocks-comments-api-openapi.yml
- filename: liveblocks-events-api-openapi.yml
  format: yaml
  label: Liveblocks Events API
  slug: liveblocks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/openapi/liveblocks-events-api-openapi.yml
- filename: liveblocks-reactions-api-openapi.yml
  format: yaml
  label: Liveblocks Reactions API
  slug: liveblocks-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/openapi/liveblocks-reactions-api-openapi.yml
- filename: liveblocks-rooms-api-openapi.yml
  format: yaml
  label: Liveblocks Rooms API
  slug: liveblocks-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/openapi/liveblocks-rooms-api-openapi.yml
- filename: liveblocks-storage-api-openapi.yml
  format: yaml
  label: Liveblocks Storage API
  slug: liveblocks-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/openapi/liveblocks-storage-api-openapi.yml
- filename: liveblocks-threads-api-openapi.yml
  format: yaml
  label: Liveblocks Threads API
  slug: liveblocks-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/openapi/liveblocks-threads-api-openapi.yml
- filename: liveblocks-versions-api-openapi.yml
  format: yaml
  label: Liveblocks Versions API
  slug: liveblocks-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/openapi/liveblocks-versions-api-openapi.yml
- filename: liveblocks-yjs-api-openapi.yml
  format: yaml
  label: Liveblocks Yjs API
  slug: liveblocks-yjs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/openapi/liveblocks-yjs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Liveblocks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Liveblocks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Liveblocks
provider_slug: liveblocks
scheme_count: 1
schemes:
- description: Authenticate with a Liveblocks secret key as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/liveblocks-openapi.yml
  type: http
slug: liveblocks-authentication
source_filename: liveblocks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/liveblocks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Authenticate with a Liveblocks secret key as a Bearer token.\n  sources:\n  - openapi/liveblocks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveblocks/refs/heads/main/authentication/liveblocks-authentication.yml
summary_line: http · 1 scheme
tags:
- Real-Time
- Collaboration
- Multiplayer
- Presence
- CRDT
- Yjs
- Comments
- Threads
- Notifications
- WebSockets
---
