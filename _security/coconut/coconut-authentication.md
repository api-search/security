---
api_key_in: []
api_specs:
- filename: coconut-openapi.yml
  format: yaml
  label: Coconut Jobs API
  slug: coconut-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coconut/refs/heads/main/openapi/coconut-openapi.yml
- filename: coconut-openapi.yml
  format: yaml
  label: Coconut Metadata API
  slug: coconut-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coconut/refs/heads/main/openapi/coconut-openapi.yml
- filename: coconut-openapi.yml
  format: yaml
  label: Coconut Webhooks API
  slug: coconut-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coconut/refs/heads/main/openapi/coconut-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Coconut Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coconut secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coconut
provider_slug: coconut
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Use the API key as the username and leave the password blank.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/coconut-openapi.yml
  type: http
slug: coconut-authentication
source_filename: coconut-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coconut-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Use the API key as the username and leave the password\n    blank.\n  sources:\n  - openapi/coconut-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coconut/refs/heads/main/authentication/coconut-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Audio
- Encoding
- Transcoding
- Media
---
