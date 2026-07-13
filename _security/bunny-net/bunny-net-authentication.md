---
api_key_in:
- header
api_specs:
- filename: bunny-net-openapi.yml
  format: yaml
  label: Bunny.net Core Platform API
  slug: core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-openapi.yml
- filename: bunny-net-stream-webhooks-asyncapi.yml
  format: yaml
  label: Bunny.net Stream Webhooks
  slug: stream-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/asyncapi/bunny-net-stream-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bunny Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bunny.net secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bunny.net
provider_slug: bunny-net
scheme_count: 1
schemes:
- description: API key issued from the Bunny.net dashboard.
  in: header
  name: accessKeyAuth
  parameter: AccessKey
  sources:
  - openapi/bunny-net-openapi.yml
  type: apiKey
slug: bunny-net-authentication
source_filename: bunny-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bunny-net-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessKeyAuth\n  type: apiKey\n  in: header\n  parameter: AccessKey\n  description: API key issued from the Bunny.net dashboard.\n  sources:\n  - openapi/bunny-net-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/authentication/bunny-net-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CDN
- Edge
- Video
- Storage
- DNS
- WAF
- Edge Compute
- Image Optimization
---
