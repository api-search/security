---
api_key_in:
- header
api_specs:
- filename: amazon-elasticache-openapi.yml
  format: yaml
  label: Amazon ElastiCache API
  slug: amazon-elasticache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-elasticache/refs/heads/main/openapi/amazon-elasticache-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Elasticache Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon ElastiCache secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon ElastiCache
provider_slug: amazon-elasticache
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-elasticache-openapi.yml
  type: apiKey
slug: amazon-elasticache-authentication
source_filename: amazon-elasticache-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-elasticache-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-elasticache-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-elasticache/refs/heads/main/authentication/amazon-elasticache-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Caching
- Database
- ElastiCache
- In-Memory
- Memcached
- Redis
---
