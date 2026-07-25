---
api_key_in: []
api_specs:
- filename: paragraph-analytics-api-openapi.yml
  format: yaml
  label: Paragraph analytics API
  slug: paragraph-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-analytics-api-openapi.yml
- filename: paragraph-auth-api-openapi.yml
  format: yaml
  label: Paragraph auth API
  slug: paragraph-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-auth-api-openapi.yml
- filename: paragraph-coins-api-openapi.yml
  format: yaml
  label: Paragraph coins API
  slug: paragraph-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-coins-api-openapi.yml
- filename: paragraph-discover-api-openapi.yml
  format: yaml
  label: Paragraph discover API
  slug: paragraph-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-discover-api-openapi.yml
- filename: paragraph-emails-api-openapi.yml
  format: yaml
  label: Paragraph emails API
  slug: paragraph-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-emails-api-openapi.yml
- filename: paragraph-me-api-openapi.yml
  format: yaml
  label: Paragraph me API
  slug: paragraph-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-me-api-openapi.yml
- filename: paragraph-posts-api-openapi.yml
  format: yaml
  label: Paragraph posts API
  slug: paragraph-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-posts-api-openapi.yml
- filename: paragraph-publications-api-openapi.yml
  format: yaml
  label: Paragraph publications API
  slug: paragraph-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-publications-api-openapi.yml
- filename: paragraph-subscribers-api-openapi.yml
  format: yaml
  label: Paragraph subscribers API
  slug: paragraph-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-subscribers-api-openapi.yml
- filename: paragraph-users-api-openapi.yml
  format: yaml
  label: Paragraph users API
  slug: paragraph-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paragraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paragraph secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paragraph
provider_slug: paragraph
scheme_count: 1
schemes:
- description: API key for authenticating protected endpoints. Pass as Bearer token in Authorization header.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/paragraph-openapi-original.json
  type: http
slug: paragraph-authentication
source_filename: paragraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/paragraph-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key for authenticating protected endpoints. Pass as Bearer token in Authorization\n    header.\n  sources:\n  - openapi/paragraph-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/authentication/paragraph-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Publishing
- Newsletters
- Web3
- Content
- Blogging
- Creator Economy
- API
---
