---
api_key_in:
- header
api_specs:
- filename: slab-openapi.yml
  format: yaml
  label: Slab Posts
  slug: posts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/openapi/slab-openapi.yml
- filename: slab-openapi.yml
  format: yaml
  label: Slab Topics
  slug: topics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/openapi/slab-openapi.yml
- filename: slab-openapi.yml
  format: yaml
  label: Slab Users
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/openapi/slab-openapi.yml
- filename: slab-openapi.yml
  format: yaml
  label: Slab Organization
  slug: organization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/openapi/slab-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Slab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Slab secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Slab
provider_slug: slab
scheme_count: 1
schemes:
- description: API token generated in Slab under Team Settings -> Developer Tools, sent in the Authorization header.
  in: header
  name: SlabToken
  parameter: Authorization
  sources:
  - openapi/slab-openapi.yml
  type: apiKey
slug: slab-authentication
source_filename: slab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/slab-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SlabToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API token generated in Slab under Team Settings -> Developer Tools, sent in the\n    Authorization header.\n  sources:\n  - openapi/slab-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/authentication/slab-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Knowledge Base
- Wiki
- Documentation
- Collaboration
- GraphQL
---
