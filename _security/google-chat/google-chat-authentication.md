---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-chat-spaces-api-openapi.yml
  format: yaml
  label: Google Chat Spaces API
  slug: google-chat-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat/openapi/google-chat-spaces-api-openapi.yml
- filename: google-chat-media-api-openapi.yml
  format: yaml
  label: Google Chat Chat Media API
  slug: google-chat-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat/openapi/google-chat-media-api-openapi.yml
- filename: google-chat-users-api-openapi.yml
  format: yaml
  label: Google Chat Chat Users API
  slug: google-chat-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat/openapi/google-chat-users-api-openapi.yml
- filename: google-chat-custom-emojis-api-openapi.yml
  format: yaml
  label: Google Chat Custom Emojis API
  slug: google-chat-custom-emojis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat/openapi/google-chat-custom-emojis-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Chat Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Chat secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Chat
provider_slug: google-chat
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-chat-custom-emojis-api-openapi.yml
  - openapi/google-chat-media-api-openapi.yml
  - openapi/google-chat-spaces-api-openapi.yml
  - openapi/google-chat-users-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 41
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-chat-custom-emojis-api-openapi.yml
  - openapi/google-chat-media-api-openapi.yml
  - openapi/google-chat-spaces-api-openapi.yml
  - openapi/google-chat-users-api-openapi.yml
  type: oauth2
slug: google-chat-authentication
source_filename: google-chat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-chat-custom-emojis-api-openapi.yml, openapi/google-chat-media-api-openapi.yml,\n  openapi/google-chat-spaces-api-openapi.yml, openapi/google-chat-users-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-chat-custom-emojis-api-openapi.yml\n  - openapi/google-chat-media-api-openapi.yml\n  - openapi/google-chat-spaces-api-openapi.yml\n  - openapi/google-chat-users-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 41\n  sources:\n  - openapi/google-chat-custom-emojis-api-openapi.yml\n  - openapi/google-chat-media-api-openapi.yml\n\
  \  - openapi/google-chat-spaces-api-openapi.yml\n  - openapi/google-chat-users-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-chat/authentication/google-chat-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Chat
- Collaboration
- Google
- Google Workspace
- Messaging
- Spaces
---
