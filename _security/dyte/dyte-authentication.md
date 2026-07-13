---
api_key_in: []
api_specs:
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Meetings API
  slug: meetings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Participants API
  slug: participants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Sessions API
  slug: sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Recordings API
  slug: recordings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Livestreams API
  slug: livestreams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
- filename: dyte-openapi.yml
  format: yaml
  label: Dyte Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/openapi/dyte-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dyte Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dyte secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dyte
provider_slug: dyte
scheme_count: 1
schemes:
- description: HTTP Basic auth using the base64-encoded string organizationId:apiKey (organizationId as the username, apiKey as the password).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/dyte-openapi.yml
  type: http
slug: dyte-authentication
source_filename: dyte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dyte-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using the base64-encoded string organizationId:apiKey (organizationId\n    as the username, apiKey as the password).\n  sources:\n  - openapi/dyte-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyte/refs/heads/main/authentication/dyte-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Voice
- Real Time
- WebRTC
- SDK
- Communications
---
