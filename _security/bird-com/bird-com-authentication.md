---
api_key_in:
- header
api_specs:
- filename: bird-com-openapi.yml
  format: yaml
  label: Bird Channels / Messaging API
  slug: bird-channels-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
- filename: bird-com-openapi.yml
  format: yaml
  label: Bird Contacts API
  slug: bird-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
- filename: bird-com-openapi.yml
  format: yaml
  label: Bird Conversations API
  slug: bird-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
- filename: bird-com-openapi.yml
  format: yaml
  label: Bird Numbers API
  slug: bird-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
- filename: bird-com-openapi.yml
  format: yaml
  label: Legacy MessageBird REST API
  slug: bird-legacy-messagebird-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bird Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bird secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bird
provider_slug: bird-com
scheme_count: 1
schemes:
- description: AccessKey token. Send as the Authorization header value "AccessKey {your-access-key}".
  in: header
  name: AccessKey
  parameter: Authorization
  sources:
  - openapi/bird-com-openapi.yml
  type: apiKey
slug: bird-com-authentication
source_filename: bird-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bird-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AccessKey token. Send as the Authorization header value \"AccessKey {your-access-key}\".\n  sources:\n  - openapi/bird-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/authentication/bird-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CRM
- Messaging
- SMS
- WhatsApp
- Email
- Voice
- Omnichannel
- CPaaS
---
