---
api_key_in: []
api_specs:
- filename: openreplay-openapi.yml
  format: yaml
  label: OpenReplay API
  slug: openreplay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/openapi/openreplay-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openreplay Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenReplay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenReplay
provider_slug: openreplay
scheme_count: 1
schemes:
- description: Organization API key from Preferences > Account > Organization API Key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openreplay-openapi.yml
  type: http
slug: openreplay-authentication
source_filename: openreplay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openreplay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Organization API key from Preferences > Account > Organization API Key.\n  sources:\n  - openapi/openreplay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/authentication/openreplay-authentication.yml
summary_line: http · 1 scheme
tags:
- Debugging
- Error Tracking
- Open Source
- Performance Monitoring
- Session Replay
- User Behavior
---
