---
api_key_in: []
api_specs:
- filename: gitclear-api-tokens-api-openapi.yml
  format: yaml
  label: GitClear API Tokens API
  slug: gitclear-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-api-tokens-api-openapi.yml
- filename: gitclear-code-introspection-api-openapi.yml
  format: yaml
  label: GitClear Code Introspection API
  slug: gitclear-code-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-code-introspection-api-openapi.yml
- filename: gitclear-data-audit-api-openapi.yml
  format: yaml
  label: GitClear Data Audit API
  slug: gitclear-data-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-data-audit-api-openapi.yml
- filename: gitclear-developers-api-openapi.yml
  format: yaml
  label: GitClear Developers API
  slug: gitclear-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-developers-api-openapi.yml
- filename: gitclear-imports-api-openapi.yml
  format: yaml
  label: GitClear Imports API
  slug: gitclear-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-imports-api-openapi.yml
- filename: gitclear-releases-api-openapi.yml
  format: yaml
  label: GitClear Releases API
  slug: gitclear-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-releases-api-openapi.yml
- filename: gitclear-reports-api-openapi.yml
  format: yaml
  label: GitClear Reports API
  slug: gitclear-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-reports-api-openapi.yml
- filename: gitclear-teams-api-openapi.yml
  format: yaml
  label: GitClear Teams API
  slug: gitclear-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-teams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gitclear Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitClear secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GitClear
provider_slug: gitclear
scheme_count: 1
schemes:
- description: GitClear API token passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gitclear-openapi.yml
  type: http
slug: gitclear-authentication
source_filename: gitclear-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitclear-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: GitClear API token passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/gitclear-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/authentication/gitclear-authentication.yml
summary_line: http · 1 scheme
tags:
- Code Analytics
- Commit Analytics
- Developer Productivity
- Diff Delta
- Engineering Metrics
---
