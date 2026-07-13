---
api_key_in:
- header
api_specs:
- filename: amazon-qldb-openapi.yml
  format: yaml
  label: Amazon QLDB API
  slug: amazon-qldb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/openapi/amazon-qldb-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Qldb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon QLDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon QLDB
provider_slug: amazon-qldb
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-qldb-openapi-original.yaml
  type: apiKey
slug: amazon-qldb-authentication
source_filename: amazon-qldb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-qldb-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-qldb-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/authentication/amazon-qldb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Database
- Ledger
---
