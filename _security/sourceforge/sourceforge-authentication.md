---
api_key_in:
- header
api_specs:
- filename: sourceforge-admin-api-openapi.yml
  format: yaml
  label: SourceForge Admin API
  slug: sourceforge-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-admin-api-openapi.yml
- filename: sourceforge-blog-api-openapi.yml
  format: yaml
  label: SourceForge Blog API
  slug: sourceforge-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-blog-api-openapi.yml
- filename: sourceforge-discussion-api-openapi.yml
  format: yaml
  label: SourceForge Discussion API
  slug: sourceforge-discussion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-discussion-api-openapi.yml
- filename: sourceforge-projects-api-openapi.yml
  format: yaml
  label: SourceForge Projects API
  slug: sourceforge-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-projects-api-openapi.yml
- filename: sourceforge-tracker-api-openapi.yml
  format: yaml
  label: SourceForge Tracker API
  slug: sourceforge-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-tracker-api-openapi.yml
- filename: sourceforge-users-api-openapi.yml
  format: yaml
  label: SourceForge Users API
  slug: sourceforge-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-users-api-openapi.yml
- filename: sourceforge-wikis-api-openapi.yml
  format: yaml
  label: SourceForge Wikis API
  slug: sourceforge-wikis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-wikis-api-openapi.yml
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
- Open-Source
- Developer Tools
- Project Management
- Code Hosting
- Collaboration
---
