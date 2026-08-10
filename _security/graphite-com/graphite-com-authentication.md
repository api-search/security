---
api_key_in: []
api_specs:
- filename: graphite-com-authentication-api-openapi.yml
  format: yaml
  label: Graphite Authentication API
  slug: graphite-com-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/openapi/graphite-com-authentication-api-openapi.yml
- filename: graphite-com-github-app-api-openapi.yml
  format: yaml
  label: Graphite GitHub App API
  slug: graphite-com-github-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/openapi/graphite-com-github-app-api-openapi.yml
- filename: graphite-com-merge-queue-api-openapi.yml
  format: yaml
  label: Graphite Merge Queue API
  slug: graphite-com-merge-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/openapi/graphite-com-merge-queue-api-openapi.yml
- filename: graphite-com-stacks-api-openapi.yml
  format: yaml
  label: Graphite Stacks API
  slug: graphite-com-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/openapi/graphite-com-stacks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Graphite Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graphite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Graphite
provider_slug: graphite-com
scheme_count: 1
schemes:
- description: Graphite auth token registered via `gt auth`, used by the CLI to act on the user's behalf.
  name: graphiteAuthToken
  scheme: bearer
  sources:
  - openapi/graphite-com-openapi.yml
  type: http
slug: graphite-com-authentication
source_filename: graphite-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/graphite-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: graphiteAuthToken\n  type: http\n  scheme: bearer\n  description: Graphite auth token registered via `gt auth`, used by the CLI to act on the user's\n    behalf.\n  sources:\n  - openapi/graphite-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/authentication/graphite-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Code Review
- Stacked PRs
- Merge Queue
- AI Code Review
- Developer Tools
- GitHub
---
