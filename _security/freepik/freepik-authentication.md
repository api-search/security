---
api_key_in:
- header
api_specs:
- filename: freepik-audio-api-openapi.yml
  format: yaml
  label: Freepik Audio API
  slug: freepik-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-audio-api-openapi.yml
- filename: freepik-image-editing-api-openapi.yml
  format: yaml
  label: Freepik Image Editing API
  slug: freepik-image-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-image-editing-api-openapi.yml
- filename: freepik-image-generation-api-openapi.yml
  format: yaml
  label: Freepik Image Generation API
  slug: freepik-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-image-generation-api-openapi.yml
- filename: freepik-resources-api-openapi.yml
  format: yaml
  label: Freepik Resources API
  slug: freepik-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-resources-api-openapi.yml
- filename: freepik-tasks-api-openapi.yml
  format: yaml
  label: Freepik Tasks API
  slug: freepik-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-tasks-api-openapi.yml
- filename: freepik-video-generation-api-openapi.yml
  format: yaml
  label: Freepik Video Generation API
  slug: freepik-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-video-generation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Freepik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freepik secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freepik
provider_slug: freepik
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: x-magnific-api-key
  sources:
  - openapi/freepik-openapi.yml
  type: apiKey
slug: freepik-authentication
source_filename: freepik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freepik-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-magnific-api-key\n  sources:\n  - openapi/freepik-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/authentication/freepik-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Graphics
- Illustrations
- Image Generation
- Photos
- Video Generation
---
