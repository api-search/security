---
api_key_in: []
api_specs:
- filename: bandwidth-calls-api-openapi.yml
  format: yaml
  label: Bandwidth Calls API
  slug: bandwidth-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-calls-api-openapi.yml
- filename: bandwidth-conferences-api-openapi.yml
  format: yaml
  label: Bandwidth Conferences API
  slug: bandwidth-conferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-conferences-api-openapi.yml
- filename: bandwidth-emergency-notification-recipients-api-openapi.yml
  format: yaml
  label: Bandwidth Emergency Notification Recipients API
  slug: bandwidth-emergency-notification-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-emergency-notification-recipients-api-openapi.yml
- filename: bandwidth-endpoints-api-openapi.yml
  format: yaml
  label: Bandwidth Endpoints API
  slug: bandwidth-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-endpoints-api-openapi.yml
- filename: bandwidth-locations-api-openapi.yml
  format: yaml
  label: Bandwidth Locations API
  slug: bandwidth-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-locations-api-openapi.yml
- filename: bandwidth-media-api-openapi.yml
  format: yaml
  label: Bandwidth Media API
  slug: bandwidth-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-media-api-openapi.yml
- filename: bandwidth-messages-api-openapi.yml
  format: yaml
  label: Bandwidth Messages API
  slug: bandwidth-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-messages-api-openapi.yml
- filename: bandwidth-recordings-api-openapi.yml
  format: yaml
  label: Bandwidth Recordings API
  slug: bandwidth-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-recordings-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bandwidth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bandwidth secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bandwidth
provider_slug: bandwidth
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using your Bandwidth Dashboard API credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bandwidth-emergency-calling-api-openapi.yml
  - openapi/bandwidth-messaging-api-openapi.yml
  - openapi/bandwidth-mfa-api-openapi.yml
  - openapi/bandwidth-phone-numbers-api-openapi.yml
  - openapi/bandwidth-toll-free-verification-api-openapi.yml
  - openapi/bandwidth-voice-api-openapi.yml
  type: http
slug: bandwidth-authentication
source_filename: bandwidth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bandwidth-emergency-calling-api-openapi.yml, openapi/bandwidth-messaging-api-openapi.yml,\n  openapi/bandwidth-mfa-api-openapi.yml, openapi/bandwidth-phone-numbers-api-openapi.yml, openapi/bandwidth-toll-free-verification-api-openapi.yml,\n  openapi/bandwidth-voice-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using your Bandwidth Dashboard API credentials.\n  sources:\n  - openapi/bandwidth-emergency-calling-api-openapi.yml\n  - openapi/bandwidth-messaging-api-openapi.yml\n  - openapi/bandwidth-mfa-api-openapi.yml\n  - openapi/bandwidth-phone-numbers-api-openapi.yml\n  - openapi/bandwidth-toll-free-verification-api-openapi.yml\n  - openapi/bandwidth-voice-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/authentication/bandwidth-authentication.yml
summary_line: http · 1 scheme
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
---
