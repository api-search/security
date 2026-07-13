---
api_key_in: []
api_specs:
- filename: jetbrains-space-openapi.yml
  format: yaml
  label: JetBrains Space HTTP API
  slug: space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-space-openapi.yml
- filename: jetbrains-teamcity-openapi.yml
  format: yaml
  label: JetBrains TeamCity REST API
  slug: teamcity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-teamcity-openapi.yml
- filename: jetbrains-youtrack-openapi.yml
  format: yaml
  label: JetBrains YouTrack REST API
  slug: youtrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-youtrack-openapi.yml
- filename: jetbrains-hub-openapi.yml
  format: yaml
  label: JetBrains Hub REST API
  slug: hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-hub-openapi.yml
- filename: jetbrains-marketplace-openapi.yml
  format: yaml
  label: JetBrains Marketplace API
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/openapi/jetbrains-marketplace-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jetbrains Authentication
name_suffix: Authentication
oauth_flows: []
overview: JetBrains secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: JetBrains
provider_slug: jetbrains
scheme_count: 2
schemes:
- description: Permanent token or OAuth 2.0 Bearer Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jetbrains-hub-openapi.yml
  - openapi/jetbrains-marketplace-openapi.yml
  - openapi/jetbrains-space-openapi.yml
  - openapi/jetbrains-teamcity-openapi.yml
  - openapi/jetbrains-youtrack-openapi.yml
  type: http
- description: Username and password authentication
  name: basicAuth
  scheme: basic
  sources:
  - openapi/jetbrains-teamcity-openapi.yml
  type: http
slug: jetbrains-authentication
source_filename: jetbrains-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jetbrains-hub-openapi.yml, openapi/jetbrains-marketplace-openapi.yml, openapi/jetbrains-space-openapi.yml,\n  openapi/jetbrains-teamcity-openapi.yml, openapi/jetbrains-youtrack-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Permanent token or OAuth 2.0 Bearer Token\n  sources:\n  - openapi/jetbrains-hub-openapi.yml\n  - openapi/jetbrains-marketplace-openapi.yml\n  - openapi/jetbrains-space-openapi.yml\n  - openapi/jetbrains-teamcity-openapi.yml\n  - openapi/jetbrains-youtrack-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Username and password authentication\n  sources:\n  - openapi/jetbrains-teamcity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/authentication/jetbrains-authentication.yml
summary_line: http · 2 schemes
tags:
- CI/CD
- Developer Tools
- IDE
---
