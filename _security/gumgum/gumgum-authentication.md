---
api_key_in:
- header
api_specs:
- filename: gumgum-contextual-api-openapi.yml
  format: yaml
  label: GumGum Contextual API
  slug: gumgum-contextual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-contextual-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gumgum Authentication
name_suffix: Authentication
oauth_flows: []
overview: GumGum secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GumGum
provider_slug: gumgum
scheme_count: 1
schemes:
- description: API key issued by GumGum, sent on every request as the X-api-key request header. Documented at https://gumgum.jira.com/wiki/spaces/VDC/pages/1712095256.
  in: header
  name: apiKeyHeader
  parameter: X-api-key
  sources:
  - openapi/gumgum-contextual-api-openapi.yml
  type: apiKey
slug: gumgum-authentication
source_filename: gumgum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/gumgum-contextual-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-api-key\n  description: API key issued by GumGum, sent on every request as the X-api-key request header.\n    Documented at https://gumgum.jira.com/wiki/spaces/VDC/pages/1712095256.\n  sources:\n  - openapi/gumgum-contextual-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/authentication/gumgum-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- advertising
- adtech
- contextual-advertising
- brand-safety
- content-classification
- computer-vision
- natural-language-processing
- video-analysis
- image-analysis
- connected-tv
- header-bidding
- programmatic-advertising
- iab-taxonomy
- content-moderation
---
