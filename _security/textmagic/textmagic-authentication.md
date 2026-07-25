---
api_key_in:
- header
api_specs:
- filename: textmagic-bulk-api-openapi.yml
  format: yaml
  label: Textmagic Bulk API
  slug: textmagic-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-bulk-api-openapi.yml
- filename: textmagic-chats-api-openapi.yml
  format: yaml
  label: Textmagic Chats API
  slug: textmagic-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-chats-api-openapi.yml
- filename: textmagic-contacts-api-openapi.yml
  format: yaml
  label: Textmagic Contacts API
  slug: textmagic-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-contacts-api-openapi.yml
- filename: textmagic-lists-api-openapi.yml
  format: yaml
  label: Textmagic Lists API
  slug: textmagic-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-lists-api-openapi.yml
- filename: textmagic-messages-api-openapi.yml
  format: yaml
  label: Textmagic Messages API
  slug: textmagic-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-messages-api-openapi.yml
- filename: textmagic-numbers-api-openapi.yml
  format: yaml
  label: Textmagic Numbers API
  slug: textmagic-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-numbers-api-openapi.yml
- filename: textmagic-replies-api-openapi.yml
  format: yaml
  label: Textmagic Replies API
  slug: textmagic-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-replies-api-openapi.yml
- filename: textmagic-schedules-api-openapi.yml
  format: yaml
  label: Textmagic Schedules API
  slug: textmagic-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-schedules-api-openapi.yml
- filename: textmagic-sender-ids-api-openapi.yml
  format: yaml
  label: Textmagic Sender IDs API
  slug: textmagic-sender-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-sender-ids-api-openapi.yml
- filename: textmagic-stats-api-openapi.yml
  format: yaml
  label: Textmagic Stats API
  slug: textmagic-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-stats-api-openapi.yml
- filename: textmagic-templates-api-openapi.yml
  format: yaml
  label: Textmagic Templates API
  slug: textmagic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-templates-api-openapi.yml
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
