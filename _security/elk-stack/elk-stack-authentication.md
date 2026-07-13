---
api_key_in:
- header
api_specs:
- filename: elasticsearch-serverless-openapi.json
  format: json
  label: Elasticsearch API
  slug: elasticsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/elastic/elasticsearch-specification/main/output/openapi/elasticsearch-serverless-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elk Stack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elastic Stack (ELK Stack) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elastic Stack (ELK Stack)
provider_slug: elk-stack
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/elk-stack-openapi.yml
  type: http
- description: ApiKey <base64-encoded-id:api_key>
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/elk-stack-openapi.yml
  type: apiKey
slug: elk-stack-authentication
source_filename: elk-stack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elk-stack-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/elk-stack-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: ApiKey <base64-encoded-id:api_key>\n  sources:\n  - openapi/elk-stack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/authentication/elk-stack-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Analytics
- Logging
- Monitoring
- Observability
- Search
---
