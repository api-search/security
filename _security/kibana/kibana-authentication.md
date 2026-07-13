---
api_key_in:
- header
api_specs:
- filename: kibana-openapi-original.yml
  format: yaml
  label: Kibana API
  slug: kibana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kibana/refs/heads/main/openapi/kibana-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kibana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kibana secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kibana
provider_slug: kibana
scheme_count: 2
schemes:
- description: 'These APIs use key-based authentication. You must create an API key and use the encoded value in the request header. For example: `Authorization: ApiKey base64AccessApiKey`'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/kibana-openapi-original.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/kibana-openapi-original.yml
  type: http
slug: kibana-authentication
source_filename: kibana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kibana-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'These APIs use key-based authentication. You must create an API key and use\n    the encoded value in the request header. For example: `Authorization: ApiKey base64AccessApiKey`'\n  sources:\n  - openapi/kibana-openapi-original.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/kibana-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kibana/refs/heads/main/authentication/kibana-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Alerting
- Analytics
- Dashboards
- Elastic Stack
- Logging
- Monitoring
- Observability
- Visualization
---
