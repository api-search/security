---
api_key_in: []
api_specs:
- filename: rootly-openapi.yml
  format: yaml
  label: Rootly
  slug: rootly
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rootly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rootly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rootly
provider_slug: rootly
scheme_count: 1
schemes:
- description: 'Bearer token authentication. Pass your API token as `Authorization: Bearer YOUR-TOKEN`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rootly-openapi.yml
  type: http
slug: rootly-authentication
source_filename: rootly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rootly-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token authentication. Pass your API token as `Authorization: Bearer YOUR-TOKEN`.'\n  sources:\n  - openapi/rootly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/authentication/rootly-authentication.yml
summary_line: http · 1 scheme
tags:
- AIOps
- Incident Management
---
