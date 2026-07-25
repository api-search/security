---
api_key_in: []
api_specs:
- filename: camtasia-assets-api-openapi.yml
  format: yaml
  label: Camtasia Assets API
  slug: camtasia-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-assets-api-openapi.yml
- filename: camtasia-categories-api-openapi.yml
  format: yaml
  label: Camtasia Categories API
  slug: camtasia-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-categories-api-openapi.yml
- filename: camtasia-downloads-api-openapi.yml
  format: yaml
  label: Camtasia Downloads API
  slug: camtasia-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-downloads-api-openapi.yml
- filename: camtasia-libraries-api-openapi.yml
  format: yaml
  label: Camtasia Libraries API
  slug: camtasia-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-libraries-api-openapi.yml
- filename: camtasia-media-api-openapi.yml
  format: yaml
  label: Camtasia Media API
  slug: camtasia-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-media-api-openapi.yml
- filename: camtasia-productions-api-openapi.yml
  format: yaml
  label: Camtasia Productions API
  slug: camtasia-productions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-productions-api-openapi.yml
- filename: camtasia-projects-api-openapi.yml
  format: yaml
  label: Camtasia Projects API
  slug: camtasia-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-projects-api-openapi.yml
- filename: camtasia-recordings-api-openapi.yml
  format: yaml
  label: Camtasia Recordings API
  slug: camtasia-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-recordings-api-openapi.yml
- filename: camtasia-templates-api-openapi.yml
  format: yaml
  label: Camtasia Templates API
  slug: camtasia-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-templates-api-openapi.yml
- filename: camtasia-tracks-api-openapi.yml
  format: yaml
  label: Camtasia Tracks API
  slug: camtasia-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-tracks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Camtasia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Camtasia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Camtasia
provider_slug: camtasia
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token from TechSmith account authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/camtasia-asset-library-openapi.yml
  - openapi/camtasia-project-management-openapi.yml
  type: http
slug: camtasia-authentication
source_filename: camtasia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/camtasia-asset-library-openapi.yml, openapi/camtasia-project-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token from TechSmith account authentication\n  sources:\n  - openapi/camtasia-asset-library-openapi.yml\n  - openapi/camtasia-project-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/authentication/camtasia-authentication.yml
summary_line: http · 1 scheme
tags:
- Screen Recording
- Video Editing
- Tutorial Creation
- E-Learning
- Screencast
- oEmbed
- SDK
---
