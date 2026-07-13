---
api_key_in:
- header
api_specs:
- filename: amazon-elastic-load-balancing-openapi.yml
  format: yaml
  label: Elastic Load Balancing v2 API
  slug: elastic-load-balancing-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/openapi/amazon-elastic-load-balancing-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Elastic Load Balancing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Elastic Load Balancing secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4Auth
  parameter: Authorization
  sources:
  - openapi/amazon-elastic-load-balancing-openapi.yml
  type: apiKey
slug: amazon-elastic-load-balancing-authentication
source_filename: amazon-elastic-load-balancing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-elastic-load-balancing-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-elastic-load-balancing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/authentication/amazon-elastic-load-balancing-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
---
