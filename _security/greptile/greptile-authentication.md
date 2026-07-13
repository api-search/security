---
api_key_in:
- header
api_specs:
- filename: greptile-openapi.yml
  format: yaml
  label: Greptile Query API
  slug: greptile-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/openapi/greptile-openapi.yml
- filename: greptile-openapi.yml
  format: yaml
  label: Greptile Repositories (Indexing) API
  slug: greptile-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/openapi/greptile-openapi.yml
- filename: greptile-openapi.yml
  format: yaml
  label: Greptile Search API
  slug: greptile-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/openapi/greptile-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Greptile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Greptile secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Greptile
provider_slug: greptile
scheme_count: 2
schemes:
- description: 'Greptile API key supplied as `Authorization: Bearer <GREPTILE_API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/greptile-openapi.yml
  type: http
- description: Git provider access token (a GitHub personal access token for GitHub remotes) Greptile uses to read repository source code.
  in: header
  name: gitHubToken
  parameter: X-GitHub-Token
  sources:
  - openapi/greptile-openapi.yml
  type: apiKey
slug: greptile-authentication
source_filename: greptile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/greptile-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Greptile API key supplied as `Authorization: Bearer <GREPTILE_API_KEY>`.'\n  sources:\n  - openapi/greptile-openapi.yml\n- name: gitHubToken\n  type: apiKey\n  in: header\n  parameter: X-GitHub-Token\n  description: Git provider access token (a GitHub personal access token for GitHub remotes)\n    Greptile uses to read repository source code.\n  sources:\n  - openapi/greptile-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/authentication/greptile-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Codebase Understanding
- Code Review
- Code Search
- Developer Tools
---
