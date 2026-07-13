---
api_key_in:
- header
api_specs:
- filename: aws-braket-quantum-tasks-api-openapi.yml
  format: yaml
  label: AWS Braket Quantum Tasks API
  slug: aws-braket-quantum-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-quantum-tasks-api-openapi.yml
- filename: aws-braket-devices-api-openapi.yml
  format: yaml
  label: AWS Braket Devices API
  slug: aws-braket-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-devices-api-openapi.yml
- filename: aws-braket-hybrid-jobs-api-openapi.yml
  format: yaml
  label: AWS Braket Hybrid Jobs API
  slug: aws-braket-hybrid-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-hybrid-jobs-api-openapi.yml
- filename: aws-braket-spending-limits-api-openapi.yml
  format: yaml
  label: AWS Braket Spending Limits API
  slug: aws-braket-spending-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-spending-limits-api-openapi.yml
- filename: aws-braket-tags-api-openapi.yml
  format: yaml
  label: AWS Braket Tags API
  slug: aws-braket-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Braket Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Braket secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Braket
provider_slug: aws-braket
scheme_count: 1
schemes:
- in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-braket-devices-api-openapi.yml
  - openapi/aws-braket-hybrid-jobs-api-openapi.yml
  - openapi/aws-braket-quantum-tasks-api-openapi.yml
  - openapi/aws-braket-spending-limits-api-openapi.yml
  - openapi/aws-braket-tags-api-openapi.yml
  type: apiKey
slug: aws-braket-authentication
source_filename: aws-braket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-braket-devices-api-openapi.yml, openapi/aws-braket-hybrid-jobs-api-openapi.yml,\n  openapi/aws-braket-quantum-tasks-api-openapi.yml, openapi/aws-braket-spending-limits-api-openapi.yml,\n  openapi/aws-braket-tags-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/aws-braket-devices-api-openapi.yml\n  - openapi/aws-braket-hybrid-jobs-api-openapi.yml\n  - openapi/aws-braket-quantum-tasks-api-openapi.yml\n  - openapi/aws-braket-spending-limits-api-openapi.yml\n  - openapi/aws-braket-tags-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/authentication/aws-braket-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Quantum Computing
- QPU
- Simulator
- Hybrid Jobs
- OpenQASM
- PennyLane
- Qiskit
- Quantum
---
