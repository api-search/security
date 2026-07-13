---
api_key_in:
- cookie
api_specs:
- filename: nebraska-update-api-openapi.yml
  format: yaml
  label: Flatcar Nebraska Update API
  slug: nebraska-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flatcar-container-linux/refs/heads/main/openapi/nebraska-update-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Flatcar Container Linux Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flatcar Container Linux secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Flatcar Container Linux
provider_slug: flatcar-container-linux
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: oidcBearerAuth
  scheme: bearer
  sources:
  - openapi/nebraska-update-api-openapi.yml
  type: http
- in: cookie
  name: oidcCookieAuth
  parameter: oidc
  sources:
  - openapi/nebraska-update-api-openapi.yml
  type: apiKey
- in: cookie
  name: githubCookieAuth
  parameter: github
  sources:
  - openapi/nebraska-update-api-openapi.yml
  type: apiKey
slug: flatcar-container-linux-authentication
source_filename: flatcar-container-linux-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nebraska-update-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: oidcBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/nebraska-update-api-openapi.yml\n- name: oidcCookieAuth\n  type: apiKey\n  in: cookie\n  parameter: oidc\n  sources:\n  - openapi/nebraska-update-api-openapi.yml\n- name: githubCookieAuth\n  type: apiKey\n  in: cookie\n  parameter: github\n  sources:\n  - openapi/nebraska-update-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flatcar-container-linux/refs/heads/main/authentication/flatcar-container-linux-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Cloud Native
- Containers
- Immutable Infrastructure
- Incubating
- Linux
- Operating System
---
