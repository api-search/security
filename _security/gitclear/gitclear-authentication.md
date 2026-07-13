---
api_key_in: []
api_specs:
- filename: gitclear-openapi.yml
  format: yaml
  label: GitClear Repositories API
  slug: gitclear-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-openapi.yml
- filename: gitclear-openapi.yml
  format: yaml
  label: GitClear Commits API
  slug: gitclear-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-openapi.yml
- filename: gitclear-openapi.yml
  format: yaml
  label: GitClear Metrics & Diff Delta API
  slug: gitclear-metrics-diff-delta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-openapi.yml
- filename: gitclear-openapi.yml
  format: yaml
  label: GitClear Developers API
  slug: gitclear-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitclear/refs/heads/main/openapi/gitclear-openapi.yml
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
