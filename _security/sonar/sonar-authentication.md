---
api_key_in: []
api_specs:
- filename: sonar-issues-api-openapi.yml
  format: yaml
  label: Sonar Issues API
  slug: sonar-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/openapi/sonar-issues-api-openapi.yml
- filename: sonar-measures-api-openapi.yml
  format: yaml
  label: Sonar Measures API
  slug: sonar-measures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/openapi/sonar-measures-api-openapi.yml
- filename: sonar-organizations-api-openapi.yml
  format: yaml
  label: Sonar Organizations API
  slug: sonar-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/openapi/sonar-organizations-api-openapi.yml
- filename: sonar-projects-api-openapi.yml
  format: yaml
  label: Sonar Projects API
  slug: sonar-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/openapi/sonar-projects-api-openapi.yml
- filename: sonar-quality-gates-api-openapi.yml
  format: yaml
  label: Sonar Quality Gates API
  slug: sonar-quality-gates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/openapi/sonar-quality-gates-api-openapi.yml
- filename: sonar-user-tokens-api-openapi.yml
  format: yaml
  label: Sonar User Tokens API
  slug: sonar-user-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/openapi/sonar-user-tokens-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sonar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sonar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sonar
provider_slug: sonar
scheme_count: 1
schemes:
- description: SonarCloud user token. Generate at https://sonarcloud.io/account/security. Pass as Bearer token or as basic auth username with empty password.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sonar-sonarcloud-api-openapi.yml
  type: http
slug: sonar-authentication
source_filename: sonar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sonar-sonarcloud-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: SonarCloud user token. Generate at https://sonarcloud.io/account/security. Pass\n    as Bearer token or as basic auth username with empty password.\n  sources:\n  - openapi/sonar-sonarcloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/authentication/sonar-authentication.yml
summary_line: http · 1 scheme
tags:
- CI/CD
- Code Quality
- DevOps
- Security
- SonarCloud
- SonarQube
- Static Analysis
---
