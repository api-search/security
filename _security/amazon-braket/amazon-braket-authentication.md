---
api_key_in:
- header
api_specs:
- filename: amazon-braket-api-openapi.yml
  format: yaml
  label: Amazon Braket API
  slug: amazon-braket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-braket/refs/heads/main/openapi/amazon-braket-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Braket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Braket secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Braket
provider_slug: amazon-braket
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_iam
  parameter: Authorization
  sources:
  - openapi/amazon-braket-api-openapi.yml
  type: apiKey
slug: amazon-braket-authentication
source_filename: amazon-braket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-braket-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_iam\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-braket-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-braket/refs/heads/main/authentication/amazon-braket-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Quantum Computing
- Quantum Hardware
- Hybrid Quantum-Classical
- QPU
- Quantum Simulation
- Amazon Web Services
- Research
- HPC
---
