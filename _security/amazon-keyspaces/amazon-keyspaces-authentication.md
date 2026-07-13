---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Keyspaces API
  slug: amazon-keyspaces-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/keyspaces/2022-02-10/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Keyspaces Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Keyspaces secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Keyspaces
provider_slug: amazon-keyspaces
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-keyspaces-openapi.yml
  type: apiKey
slug: amazon-keyspaces-authentication
source_filename: amazon-keyspaces-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-keyspaces-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-keyspaces-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-keyspaces/refs/heads/main/authentication/amazon-keyspaces-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cassandra
- Database
- Managed Database
- NoSQL
- Wide Column
---
