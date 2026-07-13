---
api_key_in: []
api_specs:
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Video Generation API
  slug: video-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Avatars / Presenters API
  slug: avatars-presenters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Job Status / Webhooks API
  slug: job-status-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Colossyan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Colossyan secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Colossyan
provider_slug: colossyan
scheme_count: 1
schemes:
- description: Bearer token authentication. Provide the workspace API token in the Authorization header as `Bearer {token}`. The token is available in the workspace Settings and requires a Business or Enterprise plan.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/colossyan-openapi.yml
  type: http
slug: colossyan-authentication
source_filename: colossyan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/colossyan-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Provide the workspace API token in the Authorization\n    header as `Bearer {token}`. The token is available in the workspace Settings and requires\n    a Business or Enterprise plan.\n  sources:\n  - openapi/colossyan-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/authentication/colossyan-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Video Generation
- Avatars
- Text to Video
- Learning and Development
---
