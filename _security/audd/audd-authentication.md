---
api_key_in:
- query
api_specs:
- filename: audd-lyrics-api-openapi.yml
  format: yaml
  label: AudD Lyrics API
  slug: audd-lyrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-lyrics-api-openapi.yml
- filename: audd-recognition-api-openapi.yml
  format: yaml
  label: AudD Recognition API
  slug: audd-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-recognition-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Audd Authentication
name_suffix: Authentication
oauth_flows: []
overview: AudD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AudD
provider_slug: audd
scheme_count: 1
schemes:
- description: API token obtained from the AudD dashboard. May also be supplied as a form field in the request body.
  in: query
  name: api_token
  parameter: api_token
  sources:
  - openapi/audd-openapi.yml
  type: apiKey
slug: audd-authentication
source_filename: audd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/audd-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: api_token\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: API token obtained from the AudD dashboard. May also be supplied as a form field\n    in the request body.\n  sources:\n  - openapi/audd-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/authentication/audd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Music
- Music Recognition
- Audio
- Fingerprinting
- Lyrics
---
