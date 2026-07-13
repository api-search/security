---
api_key_in: []
api_specs:
- filename: bandwidth-voice-api-openapi.yml
  format: yaml
  label: Bandwidth Voice API
  slug: voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-voice-api-openapi.yml
- filename: bandwidth-messaging-api-openapi.yml
  format: yaml
  label: Bandwidth Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-messaging-api-openapi.yml
- filename: bandwidth-phone-numbers-api-openapi.yml
  format: yaml
  label: Bandwidth Phone Numbers API
  slug: phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-phone-numbers-api-openapi.yml
- filename: bandwidth-mfa-api-openapi.yml
  format: yaml
  label: Bandwidth Multi-Factor Authentication API
  slug: multi-factor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-mfa-api-openapi.yml
- filename: bandwidth-emergency-calling-api-openapi.yml
  format: yaml
  label: Bandwidth Emergency Calling API
  slug: emergency-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-emergency-calling-api-openapi.yml
- filename: bandwidth-toll-free-verification-api-openapi.yml
  format: yaml
  label: Bandwidth Toll-Free Verification API
  slug: toll-free-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-toll-free-verification-api-openapi.yml
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
