---
api_key_in: []
api_specs:
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Transcriptions API
  slug: happyscribe-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Orders API
  slug: happyscribe-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Exports API
  slug: happyscribe-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Organizations API
  slug: happyscribe-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Organization Memberships API
  slug: happyscribe-organization-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Uploads API
  slug: happyscribe-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Glossaries and Style Guides API
  slug: happyscribe-glossaries-style-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Happyscribe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Happy Scribe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Happy Scribe
provider_slug: happyscribe
scheme_count: 1
schemes:
- description: 'API token from your Happy Scribe account settings, passed as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/happyscribe-openapi.yml
  type: http
slug: happyscribe-authentication
source_filename: happyscribe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/happyscribe-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token from your Happy Scribe account settings, passed as `Authorization:\n    Bearer [example key]`.'\n  sources:\n  - openapi/happyscribe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/authentication/happyscribe-authentication.yml
summary_line: http · 1 scheme
tags:
- Audio Transcription
- Transcription
- Speech-to-Text
- Subtitles
- Captions
- Translation
---
