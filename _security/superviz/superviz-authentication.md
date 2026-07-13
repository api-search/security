---
api_key_in:
- header
api_specs:
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Participants API
  slug: superviz-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Channels API
  slug: superviz-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Realtime Data API
  slug: superviz-realtime-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Rooms API
  slug: superviz-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Contextual Comments API
  slug: superviz-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Meetings API
  slug: superviz-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Webhooks API
  slug: superviz-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Authentication API
  slug: superviz-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Superviz Authentication
name_suffix: Authentication
oauth_flows: []
overview: SuperViz secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SuperViz
provider_slug: superviz
scheme_count: 2
schemes:
- description: Client ID issued from the SuperViz Dashboard under Developer > Keys. Sent on every REST request alongside the `secret` header.
  in: header
  name: clientId
  parameter: client_id
  sources:
  - openapi/superviz-openapi.yml
  type: apiKey
- description: Secret Key issued from the SuperViz Dashboard under Developer > Keys. Displayed only once at creation; store it securely and never commit it to version control.
  in: header
  name: secret
  parameter: secret
  sources:
  - openapi/superviz-openapi.yml
  type: apiKey
slug: superviz-authentication
source_filename: superviz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/superviz-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: client_id\n  description: Client ID issued from the SuperViz Dashboard under Developer > Keys. Sent on\n    every REST request alongside the `secret` header.\n  sources:\n  - openapi/superviz-openapi.yml\n- name: secret\n  type: apiKey\n  in: header\n  parameter: secret\n  description: Secret Key issued from the SuperViz Dashboard under Developer > Keys. Displayed\n    only once at creation; store it securely and never commit it to version control.\n  sources:\n  - openapi/superviz-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/authentication/superviz-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Real Time
- Collaboration
- Presence
- Synchronization
- Video
- WebRTC
- SDK
---
