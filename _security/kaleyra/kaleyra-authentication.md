---
api_key_in: []
api_specs:
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra SMS API
  slug: kaleyra-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra WhatsApp API
  slug: kaleyra-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra RCS API
  slug: kaleyra-rcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra Voice API
  slug: kaleyra-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra Verify (OTP) API
  slug: kaleyra-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra Video API
  slug: kaleyra-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kaleyra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaleyra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kaleyra
provider_slug: kaleyra
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameterName: api-key
  sources:
  - openapi/kaleyra-openapi.yml
  - https://developers.kaleyra.io/docs/generating-otp
  - https://developers.kaleyra.io/docs/click-to-call-api
  type: apiKey
slug: kaleyra-authentication
source_filename: kaleyra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/kaleyra-openapi.yml\nsummary:\n  types:\n  - apiKey\nnotes: >-\n  Kaleyra authenticates every REST request with the `api-key` HTTP header\n  carrying the API key generated in the kaleyra.io console (e.g. \"Ac4XXXXX21f\").\n  The account SID (Security Identifier) is supplied as a path segment\n  (/v2/{sid}/... or /v1/{sid}/...). There is no OAuth 2.0 flow on the core\n  messaging/voice/verify surface; Kaleyra Video issues short-lived access\n  tokens for room/participant sessions via its REST API.\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameterName: api-key\n  sources:\n  - openapi/kaleyra-openapi.yml\n  - https://developers.kaleyra.io/docs/generating-otp\n  - https://developers.kaleyra.io/docs/click-to-call-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/authentication/kaleyra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CPaaS
- Messaging
- SMS
- WhatsApp
- Voice
- OTP
- India
---
