---
api_key_in:
- header
api_specs:
- filename: kairos-ar-openapi.yml
  format: yaml
  label: Kairos Face Recognition & Emotion Analysis API
  slug: kairos-face-recognition-emotion-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kairos-ar/refs/heads/main/openapi/kairos-ar-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kairos Ar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kairos AR secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kairos AR
provider_slug: kairos-ar
scheme_count: 2
schemes:
- description: Your Kairos APP_ID, from https://developer.kairos.com.
  in: header
  name: app_id
  parameter: app_id
  sources:
  - openapi/kairos-ar-openapi.yml
  type: apiKey
- description: Your Kairos APP_KEY, from https://developer.kairos.com.
  in: header
  name: app_key
  parameter: app_key
  sources:
  - openapi/kairos-ar-openapi.yml
  type: apiKey
slug: kairos-ar-authentication
source_filename: kairos-ar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kairos-ar-openapi.yml\ndocs: https://face.kairos.com/docs/api/\nnotes: >-\n  Every request must send two apiKey headers together — app_id and app_key.\n  Keys are created and managed from the developer dashboard at\n  https://developer.kairos.com. There is no OAuth surface and no scopes.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: app_id\n  type: apiKey\n  in: header\n  parameter: app_id\n  description: Your Kairos APP_ID, from https://developer.kairos.com.\n  sources:\n  - openapi/kairos-ar-openapi.yml\n- name: app_key\n  type: apiKey\n  in: header\n  parameter: app_key\n  description: Your Kairos APP_KEY, from https://developer.kairos.com.\n  sources:\n  - openapi/kairos-ar-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kairos-ar/refs/heads/main/authentication/kairos-ar-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Face Recognition
- Facial Recognition
- Biometrics
- Emotion Analysis
- Computer Vision
- Identity
- Artificial Intelligence
- Machine Learning
- Image Analysis
---
