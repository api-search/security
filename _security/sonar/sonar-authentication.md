---
api_key_in: []
api_specs:
- filename: sonar-sonarcloud-api-openapi.yml
  format: yaml
  label: SonarCloud API
  slug: sonarcloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/openapi/sonar-sonarcloud-api-openapi.yml
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
