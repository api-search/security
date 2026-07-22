---
api_key_in:
- header
api_specs:
- filename: overops-openapi-original.json
  format: json
  label: OverOps REST API
  slug: overops-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Overops Authentication
name_suffix: Authentication
oauth_flows: []
overview: Overops secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Overops
provider_slug: overops
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/overops-openapi-original.json
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/overops-openapi-original.json
  type: apiKey
slug: overops-authentication
source_filename: overops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/overops-openapi-original.json\ndocs: https://doc.overops.com/reference\nnotes: >-\n  Confirmed against the OpenAPI info.description: authenticate with the X-API-KEY\n  header (generate under Settings -> Account Settings; recommended) or HTTP Basic\n  using a username:password combo.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/overops-openapi-original.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/overops-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/authentication/overops-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Observability
- Reliability
- Error Monitoring
- Application Performance
- Java
- DevOps
- Code Quality
---
