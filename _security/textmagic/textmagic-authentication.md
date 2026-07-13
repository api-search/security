---
api_key_in:
- header
api_specs:
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Messages API
  slug: textmagic-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Bulk Messaging API
  slug: textmagic-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Chats and Replies API
  slug: textmagic-chats-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Contacts and Lists API
  slug: textmagic-contacts-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Templates API
  slug: textmagic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Scheduled Messages API
  slug: textmagic-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Sender IDs and Numbers API
  slug: textmagic-senderids-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Textmagic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Textmagic secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Textmagic
provider_slug: textmagic
scheme_count: 2
schemes:
- description: Your Textmagic account username.
  in: header
  name: TmUsername
  parameter: X-TM-Username
  sources:
  - openapi/textmagic-openapi.yml
  type: apiKey
- description: Your Textmagic API key, generated in the account settings.
  in: header
  name: TmKey
  parameter: X-TM-Key
  sources:
  - openapi/textmagic-openapi.yml
  type: apiKey
slug: textmagic-authentication
source_filename: textmagic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/textmagic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TmUsername\n  type: apiKey\n  in: header\n  parameter: X-TM-Username\n  description: Your Textmagic account username.\n  sources:\n  - openapi/textmagic-openapi.yml\n- name: TmKey\n  type: apiKey\n  in: header\n  parameter: X-TM-Key\n  description: Your Textmagic API key, generated in the account settings.\n  sources:\n  - openapi/textmagic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/authentication/textmagic-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- SMS
- Text Messaging
- Messaging
- Communications
- CPaaS
---
