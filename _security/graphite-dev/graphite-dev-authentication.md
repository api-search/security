---
api_key_in: []
api_specs:
- filename: graphite-dev-authentication-api-openapi.yml
  format: yaml
  label: Graphite Authentication API
  slug: graphite-dev-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-authentication-api-openapi.yml
- filename: graphite-dev-github-app-api-openapi.yml
  format: yaml
  label: Graphite GitHub App API
  slug: graphite-dev-github-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-github-app-api-openapi.yml
- filename: graphite-dev-merge-queue-api-openapi.yml
  format: yaml
  label: Graphite Merge Queue API
  slug: graphite-dev-merge-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-merge-queue-api-openapi.yml
- filename: graphite-dev-stacks-api-openapi.yml
  format: yaml
  label: Graphite Stacks API
  slug: graphite-dev-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-stacks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Graphite Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graphite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Graphite
provider_slug: graphite-dev
scheme_count: 1
schemes:
- description: Graphite auth token registered via `gt auth`, used by the CLI to act on the user's behalf.
  name: graphiteAuthToken
  scheme: bearer
  sources:
  - openapi/graphite-dev-openapi.yml
  type: http
slug: graphite-dev-authentication
source_filename: graphite-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/graphite-dev-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: graphiteAuthToken\n  type: http\n  scheme: bearer\n  description: Graphite auth token registered via `gt auth`, used by the CLI to act on the user's\n    behalf.\n  sources:\n  - openapi/graphite-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/authentication/graphite-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Code Review
- Stacked PRs
- Merge Queue
- AI Code Review
- Developer Tools
- GitHub
---
