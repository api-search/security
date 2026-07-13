---
api_key_in:
- header
api_specs:
- filename: amazon-datasync-api-openapi.yml
  format: yaml
  label: Amazon DataSync REST API
  slug: amazon-datasync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/openapi/amazon-datasync-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Datasync Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon DataSync secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon DataSync
provider_slug: amazon-datasync
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-datasync-api-openapi.yml
  type: apiKey
slug: amazon-datasync-authentication
source_filename: amazon-datasync-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-datasync-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-datasync-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/authentication/amazon-datasync-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
---
