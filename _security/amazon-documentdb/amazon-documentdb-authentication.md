---
api_key_in:
- header
api_specs:
- filename: amazon-documentdb-openapi.yml
  format: yaml
  label: Amazon DocumentDB API
  slug: amazon-documentdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-documentdb/refs/heads/main/openapi/amazon-documentdb-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Documentdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DocumentDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DocumentDB
provider_slug: amazon-documentdb
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication.
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-documentdb-openapi.yml
  type: apiKey
slug: amazon-documentdb-authentication
source_filename: amazon-documentdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-documentdb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication.\n  sources:\n  - openapi/amazon-documentdb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-documentdb/refs/heads/main/authentication/amazon-documentdb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Database
- Document Database
- DocumentDB
- Managed Database
- MongoDB
- NoSQL
---
