---
api_key_in:
- header
api_specs:
- filename: amazon-panorama-application-instances-api-openapi.yml
  format: yaml
  label: Amazon Panorama Application Instances API
  slug: amazon-panorama-application-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-application-instances-api-openapi.yml
- filename: amazon-panorama-devices-api-openapi.yml
  format: yaml
  label: Amazon Panorama Devices API
  slug: amazon-panorama-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-devices-api-openapi.yml
- filename: amazon-panorama-jobs-api-openapi.yml
  format: yaml
  label: Amazon Panorama Jobs API
  slug: amazon-panorama-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-jobs-api-openapi.yml
- filename: amazon-panorama-nodes-api-openapi.yml
  format: yaml
  label: Amazon Panorama Nodes API
  slug: amazon-panorama-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-nodes-api-openapi.yml
- filename: amazon-panorama-packages-api-openapi.yml
  format: yaml
  label: Amazon Panorama Packages API
  slug: amazon-panorama-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-packages-api-openapi.yml
- filename: amazon-panorama-tags-api-openapi.yml
  format: yaml
  label: Amazon Panorama Tags API
  slug: amazon-panorama-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Panorama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Panorama secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Panorama
provider_slug: amazon-panorama
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-panorama-openapi.yml
  type: apiKey
slug: amazon-panorama-authentication
source_filename: amazon-panorama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-panorama-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-panorama-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/authentication/amazon-panorama-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Camera
- Computer-Vision
- Edge ML
- Industrial IoT
---
