---
api_key_in:
- header
api_specs:
- filename: shotstack-openapi.yml
  format: yaml
  label: Shotstack Edit (Render) API
  slug: edit-render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-openapi.yml
- filename: shotstack-openapi.yml
  format: yaml
  label: Shotstack Templates API
  slug: templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-openapi.yml
- filename: shotstack-openapi.yml
  format: yaml
  label: Shotstack Ingest API
  slug: ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-openapi.yml
- filename: shotstack-openapi.yml
  format: yaml
  label: Shotstack Serve API
  slug: serve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-openapi.yml
- filename: shotstack-openapi.yml
  format: yaml
  label: Shotstack Create (AI Assets) API
  slug: create-ai-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shotstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shotstack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shotstack
provider_slug: shotstack
scheme_count: 1
schemes:
- description: Developer API key. The same key set is used by all Shotstack APIs.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/shotstack-openapi.yml
  type: apiKey
slug: shotstack-authentication
source_filename: shotstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shotstack-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Developer API key. The same key set is used by all Shotstack APIs.\n  sources:\n  - openapi/shotstack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/authentication/shotstack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Video
- Video Editing
- Media
- Rendering
- Generative AI
---
