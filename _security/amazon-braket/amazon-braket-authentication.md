---
api_key_in:
- header
api_specs:
- filename: amazon-braket-devices-api-openapi.yml
  format: yaml
  label: Amazon Braket Devices API
  slug: amazon-braket-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-braket/refs/heads/main/openapi/amazon-braket-devices-api-openapi.yml
- filename: amazon-braket-jobs-api-openapi.yml
  format: yaml
  label: Amazon Braket Jobs API
  slug: amazon-braket-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-braket/refs/heads/main/openapi/amazon-braket-jobs-api-openapi.yml
- filename: amazon-braket-quantum-tasks-api-openapi.yml
  format: yaml
  label: Amazon Braket Quantum Tasks API
  slug: amazon-braket-quantum-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-braket/refs/heads/main/openapi/amazon-braket-quantum-tasks-api-openapi.yml
- filename: amazon-braket-spending-limits-api-openapi.yml
  format: yaml
  label: Amazon Braket Spending Limits API
  slug: amazon-braket-spending-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-braket/refs/heads/main/openapi/amazon-braket-spending-limits-api-openapi.yml
- filename: amazon-braket-tags-api-openapi.yml
  format: yaml
  label: Amazon Braket Tags API
  slug: amazon-braket-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-braket/refs/heads/main/openapi/amazon-braket-tags-api-openapi.yml
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
