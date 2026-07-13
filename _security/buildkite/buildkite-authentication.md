---
api_key_in: []
api_specs:
- filename: buildkite-openapi.yml
  format: yaml
  label: Buildkite REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Buildkite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buildkite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Buildkite
provider_slug: buildkite
scheme_count: 1
schemes:
- description: Bearer token issued from your Buildkite Personal Access Tokens page.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/buildkite-openapi.yml
  type: http
slug: buildkite-authentication
source_filename: buildkite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/buildkite-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token issued from your Buildkite Personal Access Tokens page.\n  sources:\n  - openapi/buildkite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/authentication/buildkite-authentication.yml
summary_line: http · 1 scheme
tags:
- DevOps
- CI/CD
- Pipelines
- Agents
- Self-Hosted
- GraphQL
- Test Engine
---
