---
api_key_in:
- header
api_specs:
- filename: qure.ai-fetch-results-api-openapi.yml
  format: yaml
  label: Qure.ai Fetch Results API
  slug: qure.ai-fetch-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qure.ai/refs/heads/main/openapi/qure.ai-fetch-results-api-openapi.yml
- filename: qure.ai-initiate-computation-api-openapi.yml
  format: yaml
  label: Qure.ai Initiate Computation API
  slug: qure.ai-initiate-computation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qure.ai/refs/heads/main/openapi/qure.ai-initiate-computation-api-openapi.yml
- filename: qure.ai-upload-dicoms-api-openapi.yml
  format: yaml
  label: Qure.ai Upload DICOMs API
  slug: qure.ai-upload-dicoms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qure.ai/refs/heads/main/openapi/qure.ai-upload-dicoms-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qure.Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qure.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qure.ai
provider_slug: qure.ai
scheme_count: 1
schemes:
- in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/qure.ai-platform-api-xray-ct-openapi.yml
  - openapi/qure.ai-platform-api-xray-v2-er-openapi.yml
  type: apiKey
slug: qure.ai-authentication
source_filename: qure.ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/qure.ai-platform-api-xray-ct-openapi.yml, openapi/qure.ai-platform-api-xray-v2-er-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/qure.ai-platform-api-xray-ct-openapi.yml\n  - openapi/qure.ai-platform-api-xray-v2-er-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qure.ai/refs/heads/main/authentication/qure.ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Healthcare
- Medical Imaging
- Radiology
- Machine-Learning
- DICOM
- Diagnostics
- Clinical Decision Support
- Health Technology
- Company
---
