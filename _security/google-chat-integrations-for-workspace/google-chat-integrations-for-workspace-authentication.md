---
api_key_in: []
api_specs:
- filename: google-chat-integrations-for-workspace-openapi.yml
  format: yaml
  label: Google Chat API
  slug: chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Chat Integrations For Workspace Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Chat Integrations for Workspace secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Chat Integrations for Workspace
provider_slug: google-chat-integrations-for-workspace
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-chat-integrations-for-workspace-openapi.yml
  type: oauth2
slug: google-chat-integrations-for-workspace-authentication
source_filename: google-chat-integrations-for-workspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-chat-integrations-for-workspace-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/google-chat-integrations-for-workspace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/authentication/google-chat-integrations-for-workspace-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Google Workspace
- Team Chat
- Messaging
- Collaboration
- Chat Apps
- Spaces
- Slash Commands
- Bots
---
