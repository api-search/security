---
api_key_in:
- header
api_specs:
- filename: chatwork-openapi.yml
  format: yaml
  label: Chatwork API v2
  slug: chatwork-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-openapi.yml
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
- Tasks
---
