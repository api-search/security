---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: RTB House Client Panel API
  slug: rtb-house-client-panel-api
  spec_type: OpenAPI
  url: https://api.panel.rtbhouse.com/api/docs/openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rtbhouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: RTB House secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RTB House
provider_slug: rtbhouse
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rtbhouse-client-panel-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/rtbhouse-client-panel-openapi.yml
  type: http
slug: rtbhouse-authentication
source_filename: rtbhouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rtbhouse-client-panel-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/rtbhouse-client-panel-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/rtbhouse-client-panel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/authentication/rtbhouse-authentication.yml
summary_line: http · 2 schemes
tags:
- Advertising
- Retargeting
- Programmatic
- DSP
- Deep Learning
- RTB
- Performance Marketing
---
