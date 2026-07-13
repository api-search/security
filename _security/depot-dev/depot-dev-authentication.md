---
api_key_in: []
api_specs:
- filename: depot-dev-openapi.yml
  format: yaml
  label: Depot Project API
  slug: depot-dev-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-openapi.yml
- filename: depot-dev-openapi.yml
  format: yaml
  label: Depot Build API
  slug: depot-dev-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-openapi.yml
- filename: depot-dev-openapi.yml
  format: yaml
  label: Depot BuildKit API
  slug: depot-dev-buildkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-openapi.yml
- filename: depot-dev-openapi.yml
  format: yaml
  label: Depot Tokens API
  slug: depot-dev-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Depot Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Depot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Depot
provider_slug: depot-dev
scheme_count: 1
schemes:
- description: A Depot token in the Authorization header as "Bearer {token}". Use an organization API token or user token for project/build management, and a one-time build token (from CreateBuild) for BuildKit endpoint calls.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/depot-dev-openapi.yml
  type: http
slug: depot-dev-authentication
source_filename: depot-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/depot-dev-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A Depot token in the Authorization header as \"Bearer {token}\". Use an organization\n    API token or user token for project/build management, and a one-time build token (from CreateBuild)\n    for BuildKit endpoint calls.\n  sources:\n  - openapi/depot-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/authentication/depot-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Container Builds
- Docker
- BuildKit
- Remote Cache
- CI/CD
- GitHub Actions
---
