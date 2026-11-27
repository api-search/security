---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-assistant-assistant-api-openapi.yml
  format: yaml
  label: Google Assistant API
  slug: google-assistant-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-assistant/openapi/google-assistant-assistant-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Google Assistant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Assistant declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Google Assistant
provider_slug: google-assistant
scheme_count: 1
schemes:
- flows: Google OAuth 2.0 user credentials (google-oauthlib-tool with --client-secrets)
  note: 'Docs: "Integration involves authorizing and authenticating your Google account, obtaining OAuth tokens, registering your device".'
  scopes:
  - https://www.googleapis.com/auth/assistant-sdk-prototype
  type: oauth2
slug: google-assistant-authentication
source_filename: google-assistant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Google Assistant authentication\ngenerated: '2026-11-11'\nmethod: searched\nsource: https://developers.google.com/assistant/sdk/guides/service/integrate\ndocs: https://developers.google.com/assistant/sdk/guides/service/integrate\nschemes:\n- type: oauth2\n  flows: Google OAuth 2.0 user credentials (google-oauthlib-tool with --client-secrets)\n  scopes:\n  - https://www.googleapis.com/auth/assistant-sdk-prototype\n  note: 'Docs: \"Integration involves authorizing and authenticating your Google account, obtaining OAuth tokens, registering your device\".'\n"
source_yaml_url: https://artifacts.apis.io/google-assistant/authentication/google-assistant-authentication.yml
summary_line: 1 scheme
tags:
- Actions on Google
- Conversational AI
- Google Assistant
- Natural-Language
- Smart Home
- Voice Assistant
---
