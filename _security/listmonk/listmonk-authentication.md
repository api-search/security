---
api_key_in:
- header
api_specs:
- filename: listmonk-openapi.yml
  format: yaml
  label: listmonk Subscribers API
  slug: listmonk-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-openapi.yml
- filename: listmonk-openapi.yml
  format: yaml
  label: listmonk Lists API
  slug: listmonk-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-openapi.yml
- filename: listmonk-openapi.yml
  format: yaml
  label: listmonk Campaigns API
  slug: listmonk-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-openapi.yml
- filename: listmonk-openapi.yml
  format: yaml
  label: listmonk Templates API
  slug: listmonk-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-openapi.yml
- filename: listmonk-openapi.yml
  format: yaml
  label: listmonk Media API
  slug: listmonk-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-openapi.yml
- filename: listmonk-openapi.yml
  format: yaml
  label: listmonk Transactional API
  slug: listmonk-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-openapi.yml
- filename: listmonk-openapi.yml
  format: yaml
  label: listmonk Import and Bounces API
  slug: listmonk-import-bounces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/openapi/listmonk-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Listmonk Authentication
name_suffix: Authentication
oauth_flows: []
overview: listmonk secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: listmonk
provider_slug: listmonk
scheme_count: 2
schemes:
- description: HTTP Basic auth using an API user name and token (api_user:token).
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/listmonk-openapi.yml
  type: http
- description: 'Authorization header in the form: token api_user:token.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/listmonk-openapi.yml
  type: apiKey
slug: listmonk-authentication
source_filename: listmonk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/listmonk-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using an API user name and token (api_user:token).\n  sources:\n  - openapi/listmonk-openapi.yml\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Authorization header in the form: token api_user:token.'\n  sources:\n  - openapi/listmonk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listmonk/refs/heads/main/authentication/listmonk-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email
- Newsletter
- Mailing List
- Open Source
- Self-Hosted
---
