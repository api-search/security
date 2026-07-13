---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Qiskit Runtime Jobs API
  slug: qiskit-runtime-jobs-api
  spec_type: OpenAPI
  url: https://quantum.cloud.ibm.com/api/openapi.json
- filename: ibm-quantum-runtime-backends-openapi.yml
  format: yaml
  label: Qiskit Runtime Backends API
  slug: qiskit-runtime-backends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-backends-openapi.yml
- filename: ibm-quantum-runtime-sessions-openapi.yml
  format: yaml
  label: Qiskit Runtime Sessions API
  slug: qiskit-runtime-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-sessions-openapi.yml
- filename: ibm-quantum-runtime-instances-openapi.yml
  format: yaml
  label: Qiskit Runtime Instances API
  slug: qiskit-runtime-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-instances-openapi.yml
- filename: ibm-quantum-runtime-analytics-openapi.yml
  format: yaml
  label: Qiskit Runtime Analytics API
  slug: qiskit-runtime-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-analytics-openapi.yml
- filename: ibm-quantum-runtime-versions-openapi.yml
  format: yaml
  label: Qiskit Runtime Versions API
  slug: qiskit-runtime-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-versions-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ibm Quantum Authentication
name_suffix: Authentication
oauth_flows: []
overview: ibm-quantum secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ibm-quantum
provider_slug: ibm-quantum
scheme_count: 3
schemes:
- description: IBM Cloud IAM bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ibm-quantum-runtime-analytics-openapi.yml
  - openapi/ibm-quantum-runtime-backends-openapi.yml
  - openapi/ibm-quantum-runtime-instances-openapi.yml
  - openapi/ibm-quantum-runtime-jobs-openapi.yml
  - openapi/ibm-quantum-runtime-sessions-openapi.yml
  - openapi/ibm-quantum-runtime-versions-openapi.yml
  type: http
- description: IBM Cloud Service CRN identifying the Qiskit Runtime instance
  in: header
  name: ServiceCRN
  parameter: Service-CRN
  sources:
  - openapi/ibm-quantum-runtime-analytics-openapi.yml
  - openapi/ibm-quantum-runtime-backends-openapi.yml
  - openapi/ibm-quantum-runtime-instances-openapi.yml
  - openapi/ibm-quantum-runtime-jobs-openapi.yml
  - openapi/ibm-quantum-runtime-sessions-openapi.yml
  - openapi/ibm-quantum-runtime-versions-openapi.yml
  type: apiKey
- description: API version, e.g. 2026-03-15
  in: header
  name: ApiVersion
  parameter: IBM-API-Version
  sources:
  - openapi/ibm-quantum-runtime-analytics-openapi.yml
  - openapi/ibm-quantum-runtime-backends-openapi.yml
  - openapi/ibm-quantum-runtime-instances-openapi.yml
  - openapi/ibm-quantum-runtime-jobs-openapi.yml
  - openapi/ibm-quantum-runtime-sessions-openapi.yml
  - openapi/ibm-quantum-runtime-versions-openapi.yml
  type: apiKey
slug: ibm-quantum-authentication
source_filename: ibm-quantum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ibm-quantum-runtime-analytics-openapi.yml, openapi/ibm-quantum-runtime-backends-openapi.yml,\n  openapi/ibm-quantum-runtime-instances-openapi.yml, openapi/ibm-quantum-runtime-jobs-openapi.yml,\n  openapi/ibm-quantum-runtime-sessions-openapi.yml, openapi/ibm-quantum-runtime-versions-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: IBM Cloud IAM bearer token\n  sources:\n  - openapi/ibm-quantum-runtime-analytics-openapi.yml\n  - openapi/ibm-quantum-runtime-backends-openapi.yml\n  - openapi/ibm-quantum-runtime-instances-openapi.yml\n  - openapi/ibm-quantum-runtime-jobs-openapi.yml\n  - openapi/ibm-quantum-runtime-sessions-openapi.yml\n  - openapi/ibm-quantum-runtime-versions-openapi.yml\n- name: ServiceCRN\n  type: apiKey\n  in: header\n  parameter: Service-CRN\n  description: IBM Cloud Service CRN identifying the\
  \ Qiskit Runtime instance\n  sources:\n  - openapi/ibm-quantum-runtime-analytics-openapi.yml\n  - openapi/ibm-quantum-runtime-backends-openapi.yml\n  - openapi/ibm-quantum-runtime-instances-openapi.yml\n  - openapi/ibm-quantum-runtime-jobs-openapi.yml\n  - openapi/ibm-quantum-runtime-sessions-openapi.yml\n  - openapi/ibm-quantum-runtime-versions-openapi.yml\n- name: ApiVersion\n  type: apiKey\n  in: header\n  parameter: IBM-API-Version\n  description: API version, e.g. 2026-03-15\n  sources:\n  - openapi/ibm-quantum-runtime-analytics-openapi.yml\n  - openapi/ibm-quantum-runtime-backends-openapi.yml\n  - openapi/ibm-quantum-runtime-instances-openapi.yml\n  - openapi/ibm-quantum-runtime-jobs-openapi.yml\n  - openapi/ibm-quantum-runtime-sessions-openapi.yml\n  - openapi/ibm-quantum-runtime-versions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/authentication/ibm-quantum-authentication.yml
summary_line: apiKey/http · 3 schemes
tags: []
---
