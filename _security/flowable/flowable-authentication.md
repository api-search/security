---
api_key_in: []
api_specs:
- filename: bpmn.html
  format: yaml
  label: Flowable BPMN API
  slug: flowable-bpmn-api
  spec_type: OpenAPI
  url: https://documentation.flowable.com/latest/assets/core-swagger/bpmn.html
- filename: flowable-cmmn-openapi.yml
  format: yaml
  label: Flowable CMMN API
  slug: flowable-cmmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-cmmn-openapi.yml
- filename: flowable-dmn-openapi.yml
  format: yaml
  label: Flowable DMN API
  slug: flowable-dmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-dmn-openapi.yml
- filename: flowable-form-openapi.yml
  format: yaml
  label: Flowable Form API
  slug: flowable-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-form-openapi.yml
- filename: flowable-content-openapi.yml
  format: yaml
  label: Flowable Content API
  slug: flowable-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-content-openapi.yml
- filename: flowable-idm-openapi.yml
  format: yaml
  label: Flowable IDM API
  slug: flowable-idm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-idm-openapi.yml
- filename: flowable-external-worker-openapi.yml
  format: yaml
  label: Flowable External Worker API
  slug: flowable-external-worker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-external-worker-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Flowable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flowable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flowable
provider_slug: flowable
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/flowable-bpmn-openapi.yml
  - openapi/flowable-cmmn-openapi.yml
  - openapi/flowable-content-openapi.yml
  - openapi/flowable-dmn-openapi.yml
  - openapi/flowable-external-worker-openapi.yml
  - openapi/flowable-form-openapi.yml
  - openapi/flowable-idm-openapi.yml
  type: http
slug: flowable-authentication
source_filename: flowable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flowable-bpmn-openapi.yml, openapi/flowable-cmmn-openapi.yml, openapi/flowable-content-openapi.yml,\n  openapi/flowable-dmn-openapi.yml, openapi/flowable-external-worker-openapi.yml, openapi/flowable-form-openapi.yml,\n  openapi/flowable-idm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/flowable-bpmn-openapi.yml\n  - openapi/flowable-cmmn-openapi.yml\n  - openapi/flowable-content-openapi.yml\n  - openapi/flowable-dmn-openapi.yml\n  - openapi/flowable-external-worker-openapi.yml\n  - openapi/flowable-form-openapi.yml\n  - openapi/flowable-idm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/authentication/flowable-authentication.yml
summary_line: http · 1 scheme
tags:
- BPM
- Business Process Management
- Workflow
- BPMN
- CMMN
- DMN
- Process Automation
- Case Management
- Open Source
- REST API
---
