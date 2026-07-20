---
api_key_in:
- header
api_specs:
- filename: 99designs-openapi.yml
  format: yaml
  label: 99designs API
  slug: 99designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99designs/refs/heads/main/openapi/99designs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: 99Designs Authentication
name_suffix: Authentication
oauth_flows: []
overview: 99designs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 99designs
provider_slug: 99designs
scheme_count: 2
schemes:
- in: header
  name: ApiKeyId
  parameter: Api-Key-Id
  sources:
  - openapi/99designs-openapi.yml
  type: apiKey
- in: header
  name: ApiKeySecret
  parameter: Api-Key-Secret
  sources:
  - openapi/99designs-openapi.yml
  type: apiKey
slug: 99designs-authentication
source_filename: 99designs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/99designs-openapi.yml\ndocs: https://api.99designs.com/resources/docs/\nnotes: >-\n  Authorization requires both Api-Key-Id and Api-Key-Secret headers on every\n  request. Keys are issued by 99designs after a partner requests API access at\n  https://99designs.com/api. The legacy 99designs Tasks API used HTTP Basic Auth.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyId\n  type: apiKey\n  in: header\n  parameter: Api-Key-Id\n  sources:\n  - openapi/99designs-openapi.yml\n- name: ApiKeySecret\n  type: apiKey\n  in: header\n  parameter: Api-Key-Secret\n  sources:\n  - openapi/99designs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99designs/refs/heads/main/authentication/99designs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Media
- Design
- Marketplace
- Creative
- Freelance
- Graphic Design
- Branding
---
