---
api_key_in: []
api_specs:
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Video Assets API
  slug: gumlet-video-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Video Collections API
  slug: gumlet-video-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Live Streaming API
  slug: gumlet-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Image Optimization API
  slug: gumlet-image-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Analytics API
  slug: gumlet-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Uploads API
  slug: gumlet-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gumlet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gumlet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gumlet
provider_slug: gumlet
scheme_count: 1
schemes:
- description: 'Pass your Gumlet API key as a bearer token in the Authorization header: `Authorization: Bearer <API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gumlet-openapi.yml
  type: http
slug: gumlet-authentication
source_filename: gumlet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gumlet-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Pass your Gumlet API key as a bearer token in the Authorization header: `Authorization:\n    Bearer <API_KEY>`.'\n  sources:\n  - openapi/gumlet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/authentication/gumlet-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Streaming
- Image Optimization
- CDN
- Encoding
- Analytics
---
