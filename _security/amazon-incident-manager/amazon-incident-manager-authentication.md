---
api_key_in:
- header
api_specs:
- filename: amazon-incident-manager-openapi-original.yml
  format: yaml
  label: AWS Systems Manager Incident Manager API
  slug: aws-ssm-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/openapi/amazon-incident-manager-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Incident Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Incident Manager secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-incident-manager-openapi-original.yml
  type: apiKey
slug: amazon-incident-manager-authentication
source_filename: amazon-incident-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-incident-manager-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-incident-manager-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/authentication/amazon-incident-manager-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- DevOps
- Incident Management
- Operations
---
