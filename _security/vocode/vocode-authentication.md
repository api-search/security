---
api_key_in: []
api_specs:
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Calls API
  slug: vocode-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Agents API
  slug: vocode-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Phone Numbers API
  slug: vocode-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Actions API
  slug: vocode-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Voices API
  slug: vocode-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Webhooks API
  slug: vocode-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vocode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vocode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vocode
provider_slug: vocode
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/vocode-openapi.yml
  type: http
slug: vocode-authentication
source_filename: vocode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vocode-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/vocode-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/authentication/vocode-authentication.yml
summary_line: http · 1 scheme
tags:
- Voice AI
- Voice Agents
- Telephony
- Conversational AI
- Phone Calls
---
