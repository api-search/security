---
api_key_in: []
api_specs:
- filename: freshchat-openapi.yml
  format: yaml
  label: Freshchat REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Freshchat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freshchat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freshchat
provider_slug: freshchat
scheme_count: 1
schemes:
- description: Bearer API token generated in the Freshchat admin console.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/freshchat-openapi.yml
  type: http
slug: freshchat-authentication
source_filename: freshchat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshchat-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer API token generated in the Freshchat admin console.\n  sources:\n  - openapi/freshchat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/authentication/freshchat-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Messaging
- Live Chat
- Customer Support
- Conversational Engagement
- Omnichannel Messaging
- Chatbots
- Freshworks
---
