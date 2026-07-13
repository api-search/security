---
api_key_in:
- header
api_specs:
- filename: cvat-openapi.yml
  format: yaml
  label: CVAT Projects API
  slug: cvat-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-openapi.yml
- filename: cvat-openapi.yml
  format: yaml
  label: CVAT Tasks API
  slug: cvat-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-openapi.yml
- filename: cvat-openapi.yml
  format: yaml
  label: CVAT Jobs API
  slug: cvat-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-openapi.yml
- filename: cvat-openapi.yml
  format: yaml
  label: CVAT Annotations API
  slug: cvat-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-openapi.yml
- filename: cvat-openapi.yml
  format: yaml
  label: CVAT Labels API
  slug: cvat-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-openapi.yml
- filename: cvat-openapi.yml
  format: yaml
  label: CVAT Organizations and Memberships API
  slug: cvat-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-openapi.yml
- filename: cvat-openapi.yml
  format: yaml
  label: CVAT Cloud Storages API
  slug: cvat-cloud-storages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/openapi/cvat-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cvat Authentication
name_suffix: Authentication
oauth_flows: []
overview: CVAT secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CVAT
provider_slug: cvat
scheme_count: 2
schemes:
- description: 'Token authentication. Send the header `Authorization: Token <key>` where the key is obtained from POST /auth/login.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/cvat-openapi.yml
  type: apiKey
- description: HTTP Basic authentication with CVAT username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cvat-openapi.yml
  type: http
slug: cvat-authentication
source_filename: cvat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvat-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token authentication. Send the header `Authorization: Token <key>` where the\n    key is obtained from POST /auth/login.'\n  sources:\n  - openapi/cvat-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with CVAT username and password.\n  sources:\n  - openapi/cvat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvat/refs/heads/main/authentication/cvat-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Computer Vision
- Data Annotation
- Labeling
- Datasets
- Open Source
---
