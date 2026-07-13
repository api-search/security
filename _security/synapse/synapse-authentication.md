---
api_key_in: []
api_specs:
- filename: client-server
  format: yaml
  label: Synapse Client-Server API
  slug: synapse-client-server-api
  spec_type: OpenAPI
  url: https://github.com/matrix-org/matrix-spec/tree/main/data/api/client-server
- filename: server-server
  format: yaml
  label: Synapse Server-Server API
  slug: synapse-server-server-api
  spec_type: OpenAPI
  url: https://github.com/matrix-org/matrix-spec/tree/main/data/api/server-server
- filename: synapse-admin-api-openapi.yml
  format: yaml
  label: Synapse Admin API
  slug: synapse-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/openapi/synapse-admin-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Synapse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synapse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synapse
provider_slug: synapse
scheme_count: 1
schemes:
- description: Admin access token obtained from the Synapse homeserver
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/synapse-admin-api-openapi.yml
  type: http
slug: synapse-authentication
source_filename: synapse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/synapse-admin-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Admin access token obtained from the Synapse homeserver\n  sources:\n  - openapi/synapse-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/authentication/synapse-authentication.yml
summary_line: http · 1 scheme
tags:
- Chat
- Collaboration
- Decentralized
- Federation
- Matrix
- Messaging
- Open-Source
- Real-Time
---
