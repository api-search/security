---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Slite API
  slug: slite-api
  spec_type: OpenAPI
  url: https://api.slite.com/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Slite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Slite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Slite
provider_slug: slite
scheme_count: 1
schemes:
- description: API keys can be generated under Settings > API
  name: bearer
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: slite-authentication
source_filename: slite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: API keys can be generated under Settings > API\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slite/refs/heads/main/authentication/slite-authentication.yml
summary_line: http · 1 scheme
tags:
- Documentation
- Knowledge Base
- Collaboration
- Notes
- Team
- Asynchronous Work
- AI
- Search
---
