---
api_key_in: []
api_specs:
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks SMS API
  slug: 46elks-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks MMS API
  slug: 46elks-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Voice Calls API
  slug: 46elks-voice-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Phone Numbers API
  slug: 46elks-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Media API
  slug: 46elks-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Verification API
  slug: 46elks-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 46Elks Authentication
name_suffix: Authentication
oauth_flows: []
overview: 46elks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 46elks
provider_slug: 46elks
scheme_count: 1
schemes:
- description: HTTP Basic authentication using your 46elks API username and API password from the dashboard.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/46elks-openapi.yml
  type: http
slug: 46elks-authentication
source_filename: 46elks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/46elks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using your 46elks API username and API password from\n    the dashboard.\n  sources:\n  - openapi/46elks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/authentication/46elks-authentication.yml
summary_line: http · 1 scheme
tags:
- CPaaS
- SMS
- MMS
- Voice
- Messaging
- Phone Numbers
- Communications
---
