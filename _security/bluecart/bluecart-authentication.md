---
api_key_in:
- header
api_specs:
- filename: bluecart-openapi.yml
  format: yaml
  label: BlueCart API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecart/refs/heads/main/openapi/bluecart-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bluecart Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlueCart secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BlueCart
provider_slug: bluecart
scheme_count: 2
schemes:
- description: AWS Signature Version 4 authorization against the AWS execute-api service in us-east-1. Requires an Access Key ID, Secret Access Key, and API Key generated in the BlueCart app under Settings, API Access Credentials. The API Key is supplied via the x-api-key header.
  in: header
  name: awsSigV4
  parameter: Authorization
  sources:
  - openapi/bluecart-openapi.yml
  type: apiKey
- description: BlueCart API Key generated under Settings, API Access Credentials.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/bluecart-openapi.yml
  type: apiKey
slug: bluecart-authentication
source_filename: bluecart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bluecart-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsSigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authorization against the AWS execute-api service in\n    us-east-1. Requires an Access Key ID, Secret Access Key, and API Key generated in the BlueCart\n    app under Settings, API Access Credentials. The API Key is supplied via the x-api-key header.\n  sources:\n  - openapi/bluecart-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: BlueCart API Key generated under Settings, API Access Credentials.\n  sources:\n  - openapi/bluecart-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecart/refs/heads/main/authentication/bluecart-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Restaurant
- Procurement
- Wholesale
- Ordering
- Food Distribution
- Hospitality
- eCommerce
---
