---
api_key_in:
- header
api_specs:
- filename: viam-fleet-management-api-openapi.yml
  format: yaml
  label: Viam Fleet Management API
  slug: viam-fleet-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-fleet-management-api-openapi.yml
- filename: viam-machine-management-api-openapi.yml
  format: yaml
  label: Viam Machine Management API
  slug: viam-machine-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-machine-management-api-openapi.yml
- filename: viam-data-client-api-openapi.yml
  format: yaml
  label: Viam Data Client API
  slug: viam-data-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-data-client-api-openapi.yml
- filename: viam-data-sync-api-openapi.yml
  format: yaml
  label: Viam Data Sync API
  slug: viam-data-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-data-sync-api-openapi.yml
- filename: viam-ml-training-api-openapi.yml
  format: yaml
  label: Viam ML Training API
  slug: viam-ml-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-ml-training-api-openapi.yml
- filename: viam-ml-inference-api-openapi.yml
  format: yaml
  label: Viam ML Inference API
  slug: viam-ml-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-ml-inference-api-openapi.yml
- filename: viam-billing-api-openapi.yml
  format: yaml
  label: Viam Billing API
  slug: viam-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-billing-api-openapi.yml
- filename: viam-motion-service-api-openapi.yml
  format: yaml
  label: Viam Motion Service API
  slug: viam-motion-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-motion-service-api-openapi.yml
- filename: viam-vision-service-api-openapi.yml
  format: yaml
  label: Viam Vision Service API
  slug: viam-vision-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-vision-service-api-openapi.yml
- filename: viam-slam-service-api-openapi.yml
  format: yaml
  label: Viam SLAM Service API
  slug: viam-slam-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-slam-service-api-openapi.yml
- filename: viam-ml-model-service-api-openapi.yml
  format: yaml
  label: Viam ML Model Service API
  slug: viam-ml-model-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-ml-model-service-api-openapi.yml
- filename: viam-component-apis-openapi.yml
  format: yaml
  label: Viam Component APIs
  slug: viam-component-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-component-apis-openapi.yml
- filename: viam-data-pipelines-api-openapi.yml
  format: yaml
  label: Viam Data Pipelines API
  slug: viam-data-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-data-pipelines-api-openapi.yml
- filename: viam-provisioning-api-openapi.yml
  format: yaml
  label: Viam Provisioning API
  slug: viam-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-provisioning-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Viam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Viam secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Viam
provider_slug: viam
scheme_count: 1
schemes:
- description: Viam API key.
  in: header
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/viam-billing-api-openapi.yml
  - openapi/viam-component-apis-openapi.yml
  - openapi/viam-data-client-api-openapi.yml
  - openapi/viam-data-pipelines-api-openapi.yml
  - openapi/viam-data-sync-api-openapi.yml
  - openapi/viam-fleet-management-api-openapi.yml
  - openapi/viam-machine-management-api-openapi.yml
  - openapi/viam-ml-inference-api-openapi.yml
  - openapi/viam-ml-model-service-api-openapi.yml
  - openapi/viam-ml-training-api-openapi.yml
  - openapi/viam-motion-service-api-openapi.yml
  - openapi/viam-slam-service-api-openapi.yml
  - openapi/viam-vision-service-api-openapi.yml
  type: apiKey
slug: viam-authentication
source_filename: viam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/viam-billing-api-openapi.yml, openapi/viam-component-apis-openapi.yml, openapi/viam-data-client-api-openapi.yml,\n  openapi/viam-data-pipelines-api-openapi.yml, openapi/viam-data-sync-api-openapi.yml, openapi/viam-fleet-management-api-openapi.yml,\n  openapi/viam-machine-management-api-openapi.yml, openapi/viam-ml-inference-api-openapi.yml,\n  openapi/viam-ml-model-service-api-openapi.yml, openapi/viam-ml-training-api-openapi.yml, openapi/viam-motion-service-api-openapi.yml,\n  openapi/viam-slam-service-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: key\n  description: Viam API key.\n  sources:\n  - openapi/viam-billing-api-openapi.yml\n  - openapi/viam-component-apis-openapi.yml\n  - openapi/viam-data-client-api-openapi.yml\n  - openapi/viam-data-pipelines-api-openapi.yml\n  - openapi/viam-data-sync-api-openapi.yml\n\
  \  - openapi/viam-fleet-management-api-openapi.yml\n  - openapi/viam-machine-management-api-openapi.yml\n  - openapi/viam-ml-inference-api-openapi.yml\n  - openapi/viam-ml-model-service-api-openapi.yml\n  - openapi/viam-ml-training-api-openapi.yml\n  - openapi/viam-motion-service-api-openapi.yml\n  - openapi/viam-slam-service-api-openapi.yml\n  - openapi/viam-vision-service-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/authentication/viam-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Robotics
- Edge AI
- Fleet Management
- Computer Vision
- Machine Learning
- IoT
- Embedded
- gRPC
---
