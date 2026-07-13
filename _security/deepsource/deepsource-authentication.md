---
api_key_in: []
api_specs:
- filename: deepsource-openapi.yml
  format: yaml
  label: DeepSource Repositories API
  slug: repositories
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/openapi/deepsource-openapi.yml
- filename: deepsource-openapi.yml
  format: yaml
  label: DeepSource Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/openapi/deepsource-openapi.yml
- filename: deepsource-openapi.yml
  format: yaml
  label: DeepSource Runs and Checks API
  slug: runs-checks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/openapi/deepsource-openapi.yml
- filename: deepsource-openapi.yml
  format: yaml
  label: DeepSource Analyzers API
  slug: analyzers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/openapi/deepsource-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deepsource Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeepSource secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DeepSource
provider_slug: deepsource
scheme_count: 1
schemes:
- description: 'DeepSource Personal Access Token (PAT) generated from the dashboard, passed as `Authorization: Bearer <PERSONAL_ACCESS_TOKEN>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deepsource-openapi.yml
  type: http
slug: deepsource-authentication
source_filename: deepsource-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deepsource-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'DeepSource Personal Access Token (PAT) generated from the dashboard, passed\n    as `Authorization: Bearer <PERSONAL_ACCESS_TOKEN>`.'\n  sources:\n  - openapi/deepsource-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepsource/refs/heads/main/authentication/deepsource-authentication.yml
summary_line: http · 1 scheme
tags:
- Code Quality
- Static Analysis
- Code Review
- Security
- GraphQL
---
