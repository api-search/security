---
api_key_in:
- header
api_specs:
- filename: Welcome.html
  format: yaml
  label: Amazon OpenSearch Service API
  slug: amazon-opensearch-service-api
  spec_type: OpenAPI
  url: https://docs.aws.amazon.com/opensearch-service/latest/APIReference/Welcome.html
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Opensearch Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon OpenSearch Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon OpenSearch Service
provider_slug: amazon-opensearch-service
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-opensearch-service-openapi.yml
  type: apiKey
slug: amazon-opensearch-service-authentication
source_filename: amazon-opensearch-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-opensearch-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-opensearch-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch-service/refs/heads/main/authentication/amazon-opensearch-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Elasticsearch
- Full-Text Search
- Log Analytics
- OpenSearch
- Search
---
