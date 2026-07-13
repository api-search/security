---
api_key_in: []
api_specs:
- filename: simplecast-openapi.yml
  format: yaml
  label: Simplecast Podcasts API
  slug: simplecast-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/openapi/simplecast-openapi.yml
- filename: simplecast-openapi.yml
  format: yaml
  label: Simplecast Episodes API
  slug: simplecast-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/openapi/simplecast-openapi.yml
- filename: simplecast-openapi.yml
  format: yaml
  label: Simplecast Analytics API
  slug: simplecast-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/openapi/simplecast-openapi.yml
- filename: simplecast-openapi.yml
  format: yaml
  label: Simplecast Distribution API
  slug: simplecast-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/openapi/simplecast-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Simplecast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simplecast secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Simplecast
provider_slug: simplecast
scheme_count: 1
schemes:
- description: 'Bearer token generated from the Private Apps page in the Simplecast dashboard. Sent as "authorization: Bearer {token}".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/simplecast-openapi.yml
  type: http
slug: simplecast-authentication
source_filename: simplecast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/simplecast-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token generated from the Private Apps page in the Simplecast dashboard.\n    Sent as \"authorization: Bearer {token}\".'\n  sources:\n  - openapi/simplecast-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/authentication/simplecast-authentication.yml
summary_line: http · 1 scheme
tags:
- Podcasting
- Podcast Hosting
- Podcast Distribution
- Podcast Analytics
- Audio
- Media
- SiriusXM Media
---
