---
api_key_in:
- header
api_specs:
- filename: amazon-opensearch-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API
  slug: amazon-opensearch-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/openapi/amazon-opensearch-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Opensearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon OpenSearch Service API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-opensearch-openapi.yml
  type: apiKey
slug: amazon-opensearch-authentication
source_filename: amazon-opensearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-opensearch-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-opensearch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/authentication/amazon-opensearch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Elasticsearch
- Search
---
