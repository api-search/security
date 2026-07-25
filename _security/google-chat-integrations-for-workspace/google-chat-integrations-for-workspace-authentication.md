---
api_key_in: []
api_specs:
- filename: google-chat-integrations-for-workspace-customemojis-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace CustomEmojis API
  slug: google-chat-integrations-for-workspace-customemojis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-customemojis-api-openapi.yml
- filename: google-chat-integrations-for-workspace-google-chat-api-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Google Chat API API
  slug: google-chat-integrations-for-workspace-google-chat-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-google-chat-api-api-openapi.yml
- filename: google-chat-integrations-for-workspace-members-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Members API
  slug: google-chat-integrations-for-workspace-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-members-api-openapi.yml
- filename: google-chat-integrations-for-workspace-message-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Message API
  slug: google-chat-integrations-for-workspace-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-message-api-openapi.yml
- filename: google-chat-integrations-for-workspace-messages-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Messages API
  slug: google-chat-integrations-for-workspace-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-messages-api-openapi.yml
- filename: google-chat-integrations-for-workspace-reactions-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Reactions API
  slug: google-chat-integrations-for-workspace-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-reactions-api-openapi.yml
- filename: google-chat-integrations-for-workspace-spaces-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Spaces API
  slug: google-chat-integrations-for-workspace-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml
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
