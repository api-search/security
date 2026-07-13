---
api_key_in:
- header
api_specs:
- filename: velt-openapi.yml
  format: yaml
  label: Velt Comments API
  slug: velt-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Users API
  slug: velt-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Organizations API
  slug: velt-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Documents API
  slug: velt-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Notifications API
  slug: velt-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Webhooks API
  slug: velt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Auth Tokens API
  slug: velt-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Velt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Velt secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Velt
provider_slug: velt
scheme_count: 2
schemes:
- description: Your Velt API key.
  in: header
  name: apiKeyAuth
  parameter: x-velt-api-key
  sources:
  - openapi/velt-openapi.yml
  type: apiKey
- description: Your Velt auth token that authorizes the API key.
  in: header
  name: authToken
  parameter: x-velt-auth-token
  sources:
  - openapi/velt-openapi.yml
  type: apiKey
slug: velt-authentication
source_filename: velt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/velt-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-velt-api-key\n  description: Your Velt API key.\n  sources:\n  - openapi/velt-openapi.yml\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: x-velt-auth-token\n  description: Your Velt auth token that authorizes the API key.\n  sources:\n  - openapi/velt-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/authentication/velt-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Real-Time Collaboration
- Comments
- Presence
- Notifications
- SDK
- Webhooks
---
