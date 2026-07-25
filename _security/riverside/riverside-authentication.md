---
api_key_in: []
api_specs:
- filename: riverside-exports-api-openapi.yml
  format: yaml
  label: Riverside Exports API
  slug: riverside-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riverside/refs/heads/main/openapi/riverside-exports-api-openapi.yml
- filename: riverside-productions-api-openapi.yml
  format: yaml
  label: Riverside Productions API
  slug: riverside-productions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riverside/refs/heads/main/openapi/riverside-productions-api-openapi.yml
- filename: riverside-recordings-api-openapi.yml
  format: yaml
  label: Riverside Recordings API
  slug: riverside-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riverside/refs/heads/main/openapi/riverside-recordings-api-openapi.yml
- filename: riverside-webinars-api-openapi.yml
  format: yaml
  label: Riverside Webinars API
  slug: riverside-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riverside/refs/heads/main/openapi/riverside-webinars-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Riverside Authentication
name_suffix: Authentication
oauth_flows: []
overview: Riverside secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Riverside
provider_slug: riverside
scheme_count: 1
schemes:
- description: API Key passed as Bearer token in Authorization header
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/riverside-business-openapi.yml
  type: http
slug: riverside-authentication
source_filename: riverside-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/riverside-business-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: API Key passed as Bearer token in Authorization header\n  sources:\n  - openapi/riverside-business-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riverside/refs/heads/main/authentication/riverside-authentication.yml
summary_line: http · 1 scheme
tags:
- Podcast
- Video Recording
- Media
- Content Creation
- Audio
---
