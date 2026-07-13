---
api_key_in:
- header
api_specs:
- filename: ionq-quantum-cloud-openapi.yml
  format: yaml
  label: IonQ Quantum Cloud API
  slug: ionq-quantum-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionq/refs/heads/main/openapi/ionq-quantum-cloud-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ionq Authentication
name_suffix: Authentication
oauth_flows: []
overview: IonQ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IonQ
provider_slug: ionq
scheme_count: 1
schemes:
- description: 'API keys are associated with a user and can be created on the [IonQ Quantum Cloud](https://cloud.ionq.com) application. To authenticate, prefix your API Key with `apiKey ` and place it in the `Authorization` request header. Ex: `Authorization: apiKey your-api-key`'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/ionq-quantum-cloud-openapi.yml
  type: apiKey
slug: ionq-authentication
source_filename: ionq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ionq-quantum-cloud-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API keys are associated with a user and can be created on the [IonQ Quantum\n    Cloud](https://cloud.ionq.com) application. To authenticate, prefix your API Key with `apiKey\n    ` and place it in the `Authorization` request header. Ex: `Authorization: apiKey your-api-key`'\n  sources:\n  - openapi/ionq-quantum-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ionq/refs/heads/main/authentication/ionq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Quantum Computing
- Trapped Ion
- QPU
- Aria
- Forte
- Tempo
- Quantum Cloud
- Cloud
- Hardware
- Public Company
---
