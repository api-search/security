---
api_key_in:
- header
api_specs:
- filename: amazon-directory-service-openapi.yaml
  format: yaml
  label: AWS Directory Service API
  slug: aws-directory-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/openapi/amazon-directory-service-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Directory Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Directory Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-directory-service-openapi.yaml
  type: apiKey
slug: amazon-directory-service-authentication
source_filename: amazon-directory-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-directory-service-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-directory-service-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/authentication/amazon-directory-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
---
