---
api_key_in:
- header
api_specs:
- filename: chatwork-contacts-api-openapi.yml
  format: yaml
  label: Chatwork Contacts API
  slug: chatwork-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-contacts-api-openapi.yml
- filename: chatwork-files-api-openapi.yml
  format: yaml
  label: Chatwork Files API
  slug: chatwork-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-files-api-openapi.yml
- filename: chatwork-incoming-requests-api-openapi.yml
  format: yaml
  label: Chatwork Incoming Requests API
  slug: chatwork-incoming-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-incoming-requests-api-openapi.yml
- filename: chatwork-link-api-openapi.yml
  format: yaml
  label: Chatwork Link API
  slug: chatwork-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-link-api-openapi.yml
- filename: chatwork-me-api-openapi.yml
  format: yaml
  label: Chatwork Me API
  slug: chatwork-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-me-api-openapi.yml
- filename: chatwork-members-api-openapi.yml
  format: yaml
  label: Chatwork Members API
  slug: chatwork-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-members-api-openapi.yml
- filename: chatwork-messages-api-openapi.yml
  format: yaml
  label: Chatwork Messages API
  slug: chatwork-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-messages-api-openapi.yml
- filename: chatwork-rooms-api-openapi.yml
  format: yaml
  label: Chatwork Rooms API
  slug: chatwork-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-rooms-api-openapi.yml
- filename: chatwork-tasks-api-openapi.yml
  format: yaml
  label: Chatwork Tasks API
  slug: chatwork-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-tasks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chatwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chatwork secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chatwork
provider_slug: chatwork
scheme_count: 1
schemes:
- description: API token issued from your Chatwork account settings.
  in: header
  name: chatworkToken
  parameter: X-ChatWorkToken
  sources:
  - openapi/chatwork-openapi.yml
  type: apiKey
slug: chatwork-authentication
source_filename: chatwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chatwork-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: chatworkToken\n  type: apiKey\n  in: header\n  parameter: X-ChatWorkToken\n  description: API token issued from your Chatwork account settings.\n  sources:\n  - openapi/chatwork-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/authentication/chatwork-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Messaging
- Chat
- Collaboration
- Productivity
- Task
---
