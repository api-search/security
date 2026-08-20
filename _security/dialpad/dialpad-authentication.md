---
api_key_in:
- header
api_specs:
- filename: dialpad-calls-api-openapi.yml
  format: yaml
  label: Dialpad Calls API
  slug: dialpad-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-calls-api-openapi.yml
- filename: dialpad-users-api-openapi.yml
  format: yaml
  label: Dialpad Users API
  slug: dialpad-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-users-api-openapi.yml
- filename: dialpad-asyncapi.yml
  format: yaml
  label: Dialpad Webhooks API
  slug: dialpad-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-asyncapi.yml
- filename: dialpad-calls-api-openapi.yml
  format: yaml
  label: Dialpad Calls API
  slug: dialpad-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-calls-api-openapi.yml
- filename: dialpad-contacts-api-openapi.yml
  format: yaml
  label: Dialpad Contacts API
  slug: dialpad-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-contacts-api-openapi.yml
- filename: dialpad-offices-api-openapi.yml
  format: yaml
  label: Dialpad Offices API
  slug: dialpad-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-offices-api-openapi.yml
- filename: dialpad-recordings-api-openapi.yml
  format: yaml
  label: Dialpad Recordings API
  slug: dialpad-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-recordings-api-openapi.yml
- filename: dialpad-rooms-api-openapi.yml
  format: yaml
  label: Dialpad Rooms API
  slug: dialpad-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-rooms-api-openapi.yml
- filename: dialpad-subscriptions-api-openapi.yml
  format: yaml
  label: Dialpad Subscriptions API
  slug: dialpad-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-subscriptions-api-openapi.yml
- filename: dialpad-transcripts-api-openapi.yml
  format: yaml
  label: Dialpad Transcripts API
  slug: dialpad-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-transcripts-api-openapi.yml
- filename: dialpad-users-api-openapi.yml
  format: yaml
  label: Dialpad Users API
  slug: dialpad-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-users-api-openapi.yml
- filename: dialpad-webhooks-api-openapi.yml
  format: yaml
  label: Dialpad Webhooks API
  slug: dialpad-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dialpad Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dialpad secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dialpad
provider_slug: dialpad
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dialpad-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/dialpad-openapi.yml
  type: apiKey
slug: dialpad-authentication
source_filename: dialpad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dialpad-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dialpad-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/dialpad-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/authentication/dialpad-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Communications
- Voice
- Artificial Intelligence
- Contact Center
- UCaaS
---
