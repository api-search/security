---
api_key_in: []
api_specs:
- filename: mattermost-openapi.yml
  format: yaml
  label: Mattermost REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermost/refs/heads/main/openapi/mattermost-openapi.yml
- filename: mattermost-asyncapi.yml
  format: yaml
  label: Mattermost WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermost/refs/heads/main/asyncapi/mattermost-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mattermost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mattermost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mattermost
provider_slug: mattermost
scheme_count: 1
schemes:
- description: Personal Access Token or session token issued by /users/login.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mattermost-openapi.yml
  type: http
slug: mattermost-authentication
source_filename: mattermost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mattermost-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal Access Token or session token issued by /users/login.\n  sources:\n  - openapi/mattermost-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mattermost/refs/heads/main/authentication/mattermost-authentication.yml
summary_line: http · 1 scheme
tags:
- Messaging
- Collaboration
- Team Chat
- Open Source
- DevOps
- Self-Hosted
---
