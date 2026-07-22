---
api_key_in: []
api_specs:
- filename: sonarsource-web-api-openapi.yml
  format: yaml
  label: SonarQube Cloud Web API
  slug: sonarqube-cloud-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonarsource/refs/heads/main/openapi/sonarsource-web-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sonarsource Authentication
name_suffix: Authentication
oauth_flows: []
overview: SonarSource secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SonarSource
provider_slug: sonarsource
scheme_count: 2
schemes:
- description: User token as Bearer token.
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/sonarsource-web-api-openapi.yml
  type: http
- description: User token as HTTP Basic username with empty password.
  name: basicToken
  scheme: basic
  sources:
  - openapi/sonarsource-web-api-openapi.yml
  type: http
slug: sonarsource-authentication
source_filename: sonarsource-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sonarsource-web-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: User token as Bearer token.\n  sources:\n  - openapi/sonarsource-web-api-openapi.yml\n- name: basicToken\n  type: http\n  scheme: basic\n  description: User token as HTTP Basic username with empty password.\n  sources:\n  - openapi/sonarsource-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonarsource/refs/heads/main/authentication/sonarsource-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Code Quality
- Static Analysis
- Code Security
- SAST
- Developer Tools
- DevOps
- Code Review
- SonarQube
---
