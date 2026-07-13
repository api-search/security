---
api_key_in:
- header
api_specs:
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Messaging API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Conversations API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Sequences API
  slug: sequences
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Channels API
  slug: channels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Whippy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Whippy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Whippy
provider_slug: whippy
scheme_count: 1
schemes:
- description: Organization API key. Generated in the Whippy app under Settings > Developers. OAuth 2.0 bearer tokens are also accepted via the Authorization header.
  in: header
  name: WhippyApiKey
  parameter: X-WHIPPY-KEY
  sources:
  - openapi/whippy-openapi.yml
  type: apiKey
slug: whippy-authentication
source_filename: whippy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whippy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: WhippyApiKey\n  type: apiKey\n  in: header\n  parameter: X-WHIPPY-KEY\n  description: Organization API key. Generated in the Whippy app under Settings > Developers.\n    OAuth 2.0 bearer tokens are also accepted via the Authorization header.\n  sources:\n  - openapi/whippy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/authentication/whippy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Communication
- Messaging
- SMS
- Email
- Voice
- AI
- Campaigns
- Sequences
---
