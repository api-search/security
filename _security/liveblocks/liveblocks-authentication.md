---
anonymous_access: false
api_key_in: []
api_specs:
- filename: liveblocks-comments-api-openapi.yml
  format: yaml
  label: Liveblocks Comments API
  slug: liveblocks-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-comments-api-openapi.yml
- filename: liveblocks-storage-api-openapi.yml
  format: yaml
  label: Liveblocks Storage API
  slug: liveblocks-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-storage-api-openapi.yml
- filename: liveblocks-yjs-api-openapi.yml
  format: yaml
  label: Liveblocks Yjs API
  slug: liveblocks-yjs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-yjs-api-openapi.yml
- filename: liveblocks-ai-api-openapi.yml
  format: yaml
  label: Liveblocks AI API
  slug: liveblocks-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-ai-api-openapi.yml
- filename: liveblocks-auth-api-openapi.yml
  format: yaml
  label: Liveblocks Auth API
  slug: liveblocks-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-auth-api-openapi.yml
- filename: liveblocks-feeds-api-openapi.yml
  format: yaml
  label: Liveblocks Feeds API
  slug: liveblocks-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-feeds-api-openapi.yml
- filename: liveblocks-groups-api-openapi.yml
  format: yaml
  label: Liveblocks Groups API
  slug: liveblocks-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-groups-api-openapi.yml
- filename: liveblocks-management-api-openapi.yml
  format: yaml
  label: Liveblocks Management API
  slug: liveblocks-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-management-api-openapi.yml
- filename: liveblocks-notifications-api-openapi.yml
  format: yaml
  label: Liveblocks Notifications API
  slug: liveblocks-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-notifications-api-openapi.yml
- filename: liveblocks-room-api-openapi.yml
  format: yaml
  label: Liveblocks Room API
  slug: liveblocks-room-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-room-api-openapi.yml
- filename: liveblocks-version-history-api-openapi.yml
  format: yaml
  label: Liveblocks Version History API
  slug: liveblocks-version-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-version-history-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/liveblocks/authentication/liveblocks-authentication.yml
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
- Notification
- WebSocket
---
