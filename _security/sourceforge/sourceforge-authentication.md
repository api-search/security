---
api_key_in:
- header
api_specs:
- filename: sourceforge-allura-openapi.yml
  format: yaml
  label: SourceForge Allura API
  slug: sourceforge-allura-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-allura-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sourceforge Authentication
name_suffix: Authentication
oauth_flows: []
overview: SourceForge secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SourceForge
provider_slug: sourceforge
scheme_count: 2
schemes:
- description: OAuth2 Bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sourceforge-allura-openapi.yml
  type: http
- description: OAuth 1.0 authorization header
  in: header
  name: OAuth1
  parameter: Authorization
  sources:
  - openapi/sourceforge-allura-openapi.yml
  type: apiKey
slug: sourceforge-authentication
source_filename: sourceforge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sourceforge-allura-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 Bearer token\n  sources:\n  - openapi/sourceforge-allura-openapi.yml\n- name: OAuth1\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: OAuth 1.0 authorization header\n  sources:\n  - openapi/sourceforge-allura-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/authentication/sourceforge-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Open Source
- Developer Tools
- Project Management
- Code Hosting
- Collaboration
---
