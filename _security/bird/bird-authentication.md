---
api_key_in:
- header
api_specs:
- filename: openapi-specs
  format: yaml
  label: Bird Channels API
  slug: bird-channels-api
  spec_type: OpenAPI
  url: https://github.com/messagebird/openapi-specs
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bird secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bird
provider_slug: bird
scheme_count: 1
schemes:
- description: 'Use the word "AccessKey" followed by your API Key. Example: "AccessKey w223tVQTcLO4ufBTuJxjvzwJ22"'
  in: header
  name: AccessKey
  parameter: Authorization
  sources:
  - openapi/bird-faq-openapi.yml
  - openapi/bird-intent-openapi.yml
  - openapi/bird-language-detection-openapi.yml
  - openapi/bird-ner-openapi.yml
  - openapi/bird-sms-openapi.yml
  type: apiKey
slug: bird-authentication
source_filename: bird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bird-faq-openapi.yml, openapi/bird-intent-openapi.yml, openapi/bird-language-detection-openapi.yml,\n  openapi/bird-ner-openapi.yml, openapi/bird-sms-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Use the word \"AccessKey\" followed by your API Key. Example: \"AccessKey w223tVQTcLO4ufBTuJxjvzwJ22\"'\n  sources:\n  - openapi/bird-faq-openapi.yml\n  - openapi/bird-intent-openapi.yml\n  - openapi/bird-language-detection-openapi.yml\n  - openapi/bird-ner-openapi.yml\n  - openapi/bird-sms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/authentication/bird-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Communications
- SMS
- Email
- WhatsApp
- Voice
- Messaging
- Omnichannel
- Customer Engagement
---
