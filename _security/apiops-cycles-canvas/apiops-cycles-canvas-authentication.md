---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apiops Cycles Canvas Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIOps Cycles Canvas secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIOps Cycles Canvas
provider_slug: apiops-cycles-canvas
scheme_count: 1
schemes:
- in: header
  name: apiKeys
  parameter: api-key
  sources:
  - openapi/products-api-openapi.yml
  type: apiKey
slug: apiops-cycles-canvas-authentication
source_filename: apiops-cycles-canvas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/products-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeys\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/products-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiops-cycles-canvas/refs/heads/main/authentication/apiops-cycles-canvas-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Design
- API Strategy
- Business Model
- Canvas
- Workshop
---
