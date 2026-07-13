---
api_key_in:
- header
api_specs:
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Users API
  slug: cometchat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Groups & Members API
  slug: cometchat-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Messages API
  slug: cometchat-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Conversations API
  slug: cometchat-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Roles API
  slug: cometchat-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Relationships API
  slug: cometchat-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Webhooks API
  slug: cometchat-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-asyncapi.yml
  format: yaml
  label: CometChat Realtime & Client SDK
  slug: cometchat-realtime-sdk
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/asyncapi/cometchat-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cometchat Authentication
name_suffix: Authentication
oauth_flows: []
overview: CometChat secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CometChat
provider_slug: cometchat
scheme_count: 1
schemes:
- description: Rest API Key with fullAccess scope from the CometChat dashboard. The App ID and region are encoded in the host, not in a header.
  in: header
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/cometchat-openapi.yml
  type: apiKey
slug: cometchat-authentication
source_filename: cometchat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cometchat-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Rest API Key with fullAccess scope from the CometChat dashboard. The App ID and\n    region are encoded in the host, not in a header.\n  sources:\n  - openapi/cometchat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/authentication/cometchat-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Chat
- Messaging
- Voice
- Video
- SDK
- Realtime
---
