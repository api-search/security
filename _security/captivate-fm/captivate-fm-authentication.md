---
api_key_in: []
api_specs:
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Users API
  slug: captivate-fm-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Shows API
  slug: captivate-fm-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Episodes API
  slug: captivate-fm-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Media API
  slug: captivate-fm-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Analytics API
  slug: captivate-fm-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Captivate Fm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Captivate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Captivate
provider_slug: captivate-fm
scheme_count: 1
schemes:
- description: 'Bearer token obtained from POST /authenticate/token. Sent as Authorization: Bearer {token}.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/captivate-fm-openapi.yml
  type: http
slug: captivate-fm-authentication
source_filename: captivate-fm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/captivate-fm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token obtained from POST /authenticate/token. Sent as Authorization:\n    Bearer {token}.'\n  sources:\n  - openapi/captivate-fm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/authentication/captivate-fm-authentication.yml
summary_line: http · 1 scheme
tags:
- Podcasting
- Podcast Hosting
- Episodes
- Media
- Analytics
- RSS
---
