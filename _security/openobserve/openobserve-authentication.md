---
api_key_in:
- header
api_specs:
- filename: openobserve-openapi.json
  format: json
  label: OpenObserve
  slug: openobserve
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openobserve/refs/heads/main/openapi/openobserve-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openobserve Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenObserve secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenObserve
provider_slug: openobserve
scheme_count: 2
schemes:
- in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/openobserve-openapi.json
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/openobserve-openapi.json
  type: http
slug: openobserve-authentication
source_filename: openobserve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openobserve-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/openobserve-openapi.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/openobserve-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openobserve/refs/heads/main/authentication/openobserve-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Observability
- Logs
- Metrics
- Traces
- RUM
- Open Source
---
