---
api_key_in: []
api_specs:
- filename: planable-campaigns-api-openapi.yml
  format: yaml
  label: Planable Campaigns API
  slug: planable-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-campaigns-api-openapi.yml
- filename: planable-labels-api-openapi.yml
  format: yaml
  label: Planable Labels API
  slug: planable-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-labels-api-openapi.yml
- filename: planable-media-api-openapi.yml
  format: yaml
  label: Planable Media API
  slug: planable-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-media-api-openapi.yml
- filename: planable-pages-api-openapi.yml
  format: yaml
  label: Planable Pages API
  slug: planable-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-pages-api-openapi.yml
- filename: planable-posts-api-openapi.yml
  format: yaml
  label: Planable Posts API
  slug: planable-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-posts-api-openapi.yml
- filename: planable-stories-api-openapi.yml
  format: yaml
  label: Planable Stories API
  slug: planable-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-stories-api-openapi.yml
- filename: planable-system-api-openapi.yml
  format: yaml
  label: Planable System API
  slug: planable-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-system-api-openapi.yml
- filename: planable-workspaces-api-openapi.yml
  format: yaml
  label: Planable Workspaces API
  slug: planable-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Planable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Planable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Planable
provider_slug: planable
scheme_count: 1
schemes:
- bearerFormat: pln_*
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/planable-openapi.json
  type: http
slug: planable-authentication
source_filename: planable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/planable-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: pln_*\n  sources:\n  - openapi/planable-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/authentication/planable-authentication.yml
summary_line: http · 1 scheme
tags:
- Social Media
- Content Collaboration
- Approval Workflows
- Social Media Management
- Content Publishing
- Marketing
---
