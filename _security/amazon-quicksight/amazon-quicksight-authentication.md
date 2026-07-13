---
api_key_in:
- header
api_specs:
- filename: Welcome.html
  format: yaml
  label: Amazon QuickSight API
  slug: amazon-quicksight-api
  spec_type: OpenAPI
  url: https://docs.aws.amazon.com/quicksight/latest/APIReference/Welcome.html
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Quicksight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon QuickSight secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon QuickSight
provider_slug: amazon-quicksight
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-quicksight-openapi.yml
  type: apiKey
slug: amazon-quicksight-authentication
source_filename: amazon-quicksight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-quicksight-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-quicksight-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-quicksight/refs/heads/main/authentication/amazon-quicksight-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- BI
- Business Intelligence
- Dashboards
- Machine Learning
- Reporting
- Visualization
---
