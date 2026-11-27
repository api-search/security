---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-chat-integrations-for-workspace-spaces-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Spaces API
  slug: google-chat-integrations-for-workspace-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat-integrations-for-workspace/openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml
- filename: google-chat-integrations-for-workspace-media-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Chat Integrations For Workspace Media API
  slug: google-chat-integrations-for-workspace-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat-integrations-for-workspace/openapi/google-chat-integrations-for-workspace-media-api-openapi.yml
- filename: google-chat-integrations-for-workspace-users-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Chat Integrations For Workspace Users API
  slug: google-chat-integrations-for-workspace-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat-integrations-for-workspace/openapi/google-chat-integrations-for-workspace-users-api-openapi.yml
- filename: google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Custom Emojis API
  slug: google-chat-integrations-for-workspace-custom-emojis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat-integrations-for-workspace/openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Chat Integrations for Workspace Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Chat Integrations for Workspace secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Chat Integrations for Workspace
provider_slug: google-chat-integrations-for-workspace
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml
  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml
  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml
  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 41
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml
  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml
  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml
  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml
  type: oauth2
slug: google-chat-integrations-for-workspace-authentication
source_filename: google-chat-integrations-for-workspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml, openapi/google-chat-integrations-for-workspace-media-api-openapi.yml,\n  openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml, openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n \
  \   authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 41\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-chat-integrations-for-workspace/authentication/google-chat-integrations-for-workspace-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
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
