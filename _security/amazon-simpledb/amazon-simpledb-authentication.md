---
api_key_in:
- header
api_specs:
- filename: amazon-simpledb.yaml
  format: yaml
  label: Amazon SimpleDB API
  slug: amazon-simpledb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Simpledb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon SimpleDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
scheme_count: 1
schemes:
- description: Amazon Signature authorization v2
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-simpledb.yaml
  type: apiKey
slug: amazon-simpledb-authentication
source_filename: amazon-simpledb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-simpledb.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v2\n  sources:\n  - openapi/amazon-simpledb.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/authentication/amazon-simpledb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
---
