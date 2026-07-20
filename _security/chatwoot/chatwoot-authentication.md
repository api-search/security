---
api_key_in:
- header
api_specs:
- filename: swagger.json
  format: json
  label: Chatwoot Application API
  slug: application-api
  spec_type: OpenAPI
  url: https://www.chatwoot.com/swagger/swagger.json
- filename: chatwoot-platform-apis
  format: yaml
  label: Chatwoot Platform API
  slug: platform-api
  spec_type: Postman
  url: https://www.postman.com/chatwoot/chatwoot-apis/documentation/m2zyu6l/chatwoot-platform-apis
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chatwoot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chatwoot secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chatwoot
provider_slug: chatwoot
scheme_count: 1
schemes:
- description: This token can be obtained by visiting the profile page or via rails console. Provides access to  endpoints based on the user permissions levels. This token can be saved by an external system when user is created via API, to perform activities on behalf of the user.
  in: header
  name: userApiKey
  parameter: api_access_token
  sources:
  - openapi/chatwoot-application-api-openapi.yml
  type: apiKey
slug: chatwoot-authentication
source_filename: chatwoot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chatwoot-application-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: userApiKey\n  type: apiKey\n  in: header\n  parameter: api_access_token\n  description: This token can be obtained by visiting the profile page or via rails console.\n    Provides access to  endpoints based on the user permissions levels. This token can be saved\n    by an external system when user is created via API, to perform activities on behalf of the\n    user.\n  sources:\n  - openapi/chatwoot-application-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatwoot/refs/heads/main/authentication/chatwoot-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Customer Support
- Messaging
- Live Chat
- Omni-channel
- Conversations
- Contacts
- Agents
- Open Source
---
