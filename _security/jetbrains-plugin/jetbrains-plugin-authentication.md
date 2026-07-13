---
api_key_in: []
api_specs:
- filename: jetbrains-plugin-openapi.yml
  format: yaml
  label: JetBrains Marketplace API
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains-plugin/refs/heads/main/openapi/jetbrains-plugin-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jetbrains Plugin Authentication
name_suffix: Authentication
oauth_flows: []
overview: JetBrains Marketplace secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JetBrains Marketplace
provider_slug: jetbrains-plugin
scheme_count: 1
schemes:
- bearerFormat: PermanentToken
  description: JetBrains Hub permanent token
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/jetbrains-plugin-openapi.yml
  type: http
slug: jetbrains-plugin-authentication
source_filename: jetbrains-plugin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jetbrains-plugin-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: PermanentToken\n  description: JetBrains Hub permanent token\n  sources:\n  - openapi/jetbrains-plugin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetbrains-plugin/refs/heads/main/authentication/jetbrains-plugin-authentication.yml
summary_line: http · 1 scheme
tags:
- Plugins
- IDE
- Marketplace
- Developer Tools
- JetBrains
- IntelliJ
---
