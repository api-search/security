---
api_key_in:
- header
api_specs:
- filename: sendbird-platform-openapi.yml
  format: yaml
  label: Sendbird Platform API
  slug: sendbird-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendbird/refs/heads/main/openapi/sendbird-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sendbird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sendbird secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sendbird
provider_slug: sendbird
scheme_count: 1
schemes:
- description: Sendbird master or secondary API token obtained from the Sendbird Dashboard.
  in: header
  name: apiTokenAuth
  parameter: Api-Token
  sources:
  - openapi/sendbird-platform-openapi.yml
  type: apiKey
slug: sendbird-authentication
source_filename: sendbird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/sendbird-platform-openapi.yml\ndocs: https://sendbird.com/docs/chat/platform-api/v3/prepare-to-use-api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\ntoken_model:\n  - name: master API token\n    description: Auto-generated when an application is created; cannot be revoked or modified. Sent in the Api-Token header.\n  - name: secondary API tokens\n    description: Generated and managed via the Platform API; revocable. Sent in the Api-Token header.\n  - name: session/access tokens\n    description: Per-user tokens for client-side authentication (issued via user create / token endpoints).\nguidance: >-\n  The Platform API is server-side only. Sendbird docs warn: \"DON'T send any Chat\n  API requests from your client app\" — use per-user session tokens on clients.\nschemes:\n- name: apiTokenAuth\n  type: apiKey\n  in: header\n  parameter: Api-Token\n  description: Sendbird master or secondary API token obtained\
  \ from the Sendbird Dashboard.\n  sources:\n  - openapi/sendbird-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendbird/refs/heads/main/authentication/sendbird-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
