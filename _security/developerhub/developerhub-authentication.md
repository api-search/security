---
api_key_in:
- header
api_specs:
- filename: developerhub-openapi.yml
  format: yaml
  label: DeveloperHub Documentation Platform
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Developerhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeveloperHub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DeveloperHub
provider_slug: developerhub
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/developerhub-openapi.yml
  type: apiKey
slug: developerhub-authentication
source_filename: developerhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/developerhub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/developerhub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/authentication/developerhub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Reference
- Developer Portals
- Documentation
- Knowledge Base
---
