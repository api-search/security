---
api_key_in: []
api_specs:
- filename: quora-chat-api-openapi.yml
  format: yaml
  label: Quora Chat API
  slug: quora-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quora/refs/heads/main/openapi/quora-chat-api-openapi.yml
- filename: quora-models-api-openapi.yml
  format: yaml
  label: Quora Models API
  slug: quora-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quora/refs/heads/main/openapi/quora-models-api-openapi.yml
- filename: quora-responses-api-openapi.yml
  format: yaml
  label: Quora Responses API
  slug: quora-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quora/refs/heads/main/openapi/quora-responses-api-openapi.yml
- filename: quora-usage-api-openapi.yml
  format: yaml
  label: Quora Usage API
  slug: quora-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quora/refs/heads/main/openapi/quora-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quora secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quora
provider_slug: quora
scheme_count: 1
schemes:
- description: 'Bearer token issued from https://poe.com/api/keys. Pass as `Authorization: Bearer <api_key>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/quora-poe-api-openapi.yml
  type: http
slug: quora-authentication
source_filename: quora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quora-poe-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token issued from https://poe.com/api/keys. Pass as `Authorization: Bearer\n    <api_key>`.'\n  sources:\n  - openapi/quora-poe-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quora/refs/heads/main/authentication/quora-authentication.yml
summary_line: http · 1 scheme
tags:
- Community
- Knowledge
- Q&A
---
