---
api_key_in:
- header
api_specs:
- filename: elastic-elasticsearch-openapi.yml
  format: yaml
  label: Elasticsearch REST API
  slug: elasticsearch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-elasticsearch-openapi.yml
- filename: elastic-kibana-openapi.yml
  format: yaml
  label: Kibana API
  slug: kibana
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-kibana-openapi.yml
- filename: elastic-cloud-openapi.yml
  format: yaml
  label: Elastic Cloud API
  slug: elastic-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-cloud-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elastic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elastic secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elastic
provider_slug: elastic
scheme_count: 2
schemes:
- description: ApiKey <api_key>
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/elastic-cloud-openapi.yml
  - openapi/elastic-elasticsearch-openapi.yml
  - openapi/elastic-kibana-openapi.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/elastic-elasticsearch-openapi.yml
  - openapi/elastic-kibana-openapi.yml
  type: http
slug: elastic-authentication
source_filename: elastic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elastic-cloud-openapi.yml, openapi/elastic-elasticsearch-openapi.yml, openapi/elastic-kibana-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: ApiKey <api_key>\n  sources:\n  - openapi/elastic-cloud-openapi.yml\n  - openapi/elastic-elasticsearch-openapi.yml\n  - openapi/elastic-kibana-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/elastic-elasticsearch-openapi.yml\n  - openapi/elastic-kibana-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/authentication/elastic-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Search
- Analytics
- Observability
- Security
- Visualization
- Cloud
---
