---
api_key_in: []
api_specs:
- filename: community.html
  format: yaml
  label: Common Room Core API
  slug: common-room-core-api
  spec_type: OpenAPI
  url: https://api.commonroom.io/docs/community.html
- filename: common-room-scim-openapi.yml
  format: yaml
  label: Common Room SCIM API
  slug: common-room-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/common-room/refs/heads/main/openapi/common-room-scim-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Common Room Authentication
name_suffix: Authentication
oauth_flows: []
overview: Common Room secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Common Room
provider_slug: common-room
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: "Use a Core API JWT as a Bearer token in the Authentication header.\n\nTokens can be created by room Admins through https://app.commonroom.io/\n\nExample:\n\n```\ncurl -H \"Authorization: Bearer [example key]\" \\\n  https://api.commonroom.io/community/v1/api-token-status\n````"
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/common-room-core-openapi.yml
  - openapi/common-room-scim-openapi.yml
  - openapi/common-room-v2-openapi.yml
  type: http
slug: common-room-authentication
source_filename: common-room-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/common-room-core-openapi.yml, openapi/common-room-scim-openapi.yml, openapi/common-room-v2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Use a Core API JWT as a Bearer token in the Authentication header.\n\n    Tokens can be created by room Admins through https://app.commonroom.io/\n\n    Example:\n\n    ```\n    curl -H \"Authorization: Bearer [example key]\" \\\n      https://api.commonroom.io/community/v1/api-token-status\n    ````\n  sources:\n  - openapi/common-room-core-openapi.yml\n  - openapi/common-room-scim-openapi.yml\n  - openapi/common-room-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/common-room/refs/heads/main/authentication/common-room-authentication.yml
summary_line: http · 1 scheme
tags:
- Community Intelligence
- Go-to-Market
- Member Signals
- GitHub
- Slack
- Discord
- LinkedIn
- Sales Intelligence
- Contact Management
- Webhooks
---
