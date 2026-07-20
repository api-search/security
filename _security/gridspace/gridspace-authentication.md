---
api_key_in:
- header
api_specs:
- filename: gridspace-guava-openapi.yml
  format: yaml
  label: Guava Voice Agent REST API
  slug: guava-voice-agent-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridspace/refs/heads/main/openapi/gridspace-guava-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gridspace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gridspace secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gridspace
provider_slug: gridspace
scheme_count: 2
schemes:
- applies_to: REST API, Python SDK, TypeScript SDK
  env_var: GUAVA_API_KEY
  format: Bearer [example key]
  header: Authorization
  in: header
  key_prefix: gva-
  name: bearerAuth
  provisioning: https://app.goguava.ai/dashboard/api-keys
  scheme: bearer
  sources:
  - openapi/gridspace-guava-openapi.yml
  type: http
- command: guava login
  description: Browser-based OAuth used by the guava CLI to authenticate the developer; credentials are stored locally and can be reused by the SDKs. No public OAuth scope catalog is documented.
  flow: browser-login
  headless_flag: --no-launch-browser
  name: cliOAuth
  sources:
  - https://goguava.ai/docs/cli-reference
  type: oauth2
slug: gridspace-authentication
source_filename: gridspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://goguava.ai/docs/api-overview\ndocs: https://goguava.ai/docs/sdk-installation\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The Guava REST API and SDKs authenticate with a bearer API key. The CLI uses\n    a separate browser-based OAuth login (guava login) that stores credentials\n    locally; the TypeScript and Python SDKs can reuse those CLI credentials.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer [example key]'\n  key_prefix: 'gva-'\n  env_var: GUAVA_API_KEY\n  provisioning: https://app.goguava.ai/dashboard/api-keys\n  applies_to: REST API, Python SDK, TypeScript SDK\n  sources: [openapi/gridspace-guava-openapi.yml]\n- name: cliOAuth\n  type: oauth2\n  flow: browser-login\n  command: guava login\n  headless_flag: --no-launch-browser\n  description: >-\n    Browser-based OAuth\
  \ used by the guava CLI to authenticate the developer;\n    credentials are stored locally and can be reused by the SDKs. No public\n    OAuth scope catalog is documented.\n  sources: [https://goguava.ai/docs/cli-reference]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridspace/refs/heads/main/authentication/gridspace-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Voice AI
- Conversational AI
- Voice Agents
- Speech Recognition
- Telephony
- SMS
- Contact Center
- Regulated Industries
- Healthcare
---
