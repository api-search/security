---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: frejun-teler-events-api-openapi.yml
  format: yaml
  label: FreJun Teler Events API
  slug: frejun-teler-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-events-api-openapi.yml
- filename: frejun-teler-secrets-api-openapi.yml
  format: yaml
  label: FreJun Teler Secrets API
  slug: frejun-teler-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-secrets-api-openapi.yml
- filename: frejun-teler-sip-calls-api-openapi.yml
  format: yaml
  label: FreJun Teler SIP / Calls API
  slug: frejun-teler-sip-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-sip-calls-api-openapi.yml
- filename: frejun-teler-sip-ip-access-control-lists-api-openapi.yml
  format: yaml
  label: FreJun Teler SIP / IP Access Control Lists API
  slug: frejun-teler-sip-ip-access-control-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-sip-ip-access-control-lists-api-openapi.yml
- filename: frejun-teler-sip-trunks-api-openapi.yml
  format: yaml
  label: FreJun Teler SIP / Trunks API
  slug: frejun-teler-sip-trunks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-sip-trunks-api-openapi.yml
- filename: frejun-teler-utilities-api-openapi.yml
  format: yaml
  label: FreJun Teler Utilities API
  slug: frejun-teler-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-utilities-api-openapi.yml
- filename: frejun-teler-virtual-numbers-api-openapi.yml
  format: yaml
  label: FreJun Teler Virtual Numbers API
  slug: frejun-teler-virtual-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-virtual-numbers-api-openapi.yml
- filename: frejun-teler-voice-apps-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Apps API
  slug: frejun-teler-voice-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-apps-api-openapi.yml
- filename: frejun-teler-voice-call-controls-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Call Controls API
  slug: frejun-teler-voice-call-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-call-controls-api-openapi.yml
- filename: frejun-teler-voice-calls-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Calls API
  slug: frejun-teler-voice-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-calls-api-openapi.yml
- filename: frejun-teler-voice-calls-legacy-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Calls (legacy) API
  slug: frejun-teler-voice-calls-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-calls-legacy-api-openapi.yml
- filename: frejun-teler-voice-operations-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Operations API
  slug: frejun-teler-voice-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-operations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Frejun Teler Authentication
name_suffix: Authentication
oauth_flows: []
overview: FreJun Teler secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FreJun Teler
provider_slug: frejun-teler
scheme_count: 1
schemes:
- description: Your secret account API key. Create one in the Teler dashboard.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/frejun-teler-openapi.json
  type: apiKey
slug: frejun-teler-authentication
source_filename: frejun-teler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "aid: frejun-teler\ntype: Authentication\ngenerated: '2026-09-15'\nmethod: searched\nsource: openapi/frejun-teler-openapi.json + Teler OpenAPI info.description (api.frejun.ai/openapi.json)\ndocs: https://frejun.com/docs/teler/\nnotes: >-\n  Single scheme: a secret, account-scoped API key sent in the x-api-key request\n  header. Keys grant full account access (treat like a password, keep\n  server-side, rotate from the Teler dashboard at platform.frejun.ai). A missing\n  or invalid key returns HTTP 403. No OAuth2/OIDC on the developer API.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Your secret account API key. Create one in the Teler dashboard.\n  sources:\n  - openapi/frejun-teler-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/authentication/frejun-teler-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- programmable voice API
- voice AI infrastructure
- CPaaS
- SIP Trunking
- telephony API
- real-time media streaming
- WebSocket audio
- Call Automation
- conversational AI infrastructure
---
