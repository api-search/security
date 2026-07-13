---
api_key_in:
- header
api_specs:
- filename: elsa-openapi.yml
  format: yaml
  label: ELSA Pronunciation Assessment API (Scripted)
  slug: elsa-pronunciation-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsa/refs/heads/main/openapi/elsa-openapi.yml
- filename: elsa-openapi.yml
  format: yaml
  label: ELSA Realtime Streaming Speech API
  slug: elsa-realtime-streaming-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsa/refs/heads/main/openapi/elsa-openapi.yml
- filename: elsa-openapi.yml
  format: yaml
  label: ELSA Unscripted Speech Assessment API
  slug: elsa-unscripted-speech-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsa/refs/heads/main/openapi/elsa-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Elsa Authentication
name_suffix: Authentication
oauth_flows: []
overview: ELSA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ELSA
provider_slug: elsa
scheme_count: 1
schemes:
- description: 'API token passed in the Authorization header using the ELSA scheme, e.g. "Authorization: ELSA <API_token>". Tokens are issued to partners; an optional master key can generate tokens programmatically. Request access via the ELSA website.'
  in: header
  name: ElsaAuth
  parameter: Authorization
  sources:
  - openapi/elsa-openapi.yml
  type: apiKey
slug: elsa-authentication
source_filename: elsa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elsa-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ElsaAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API token passed in the Authorization header using the ELSA scheme, e.g. \"Authorization:\n    ELSA <API_token>\". Tokens are issued to partners; an optional master key can generate tokens\n    programmatically. Request access via the ELSA website.'\n  sources:\n  - openapi/elsa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elsa/refs/heads/main/authentication/elsa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Speech Assessment
- Pronunciation
- Speech Recognition
- Language Learning
- AI
---
