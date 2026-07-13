---
api_key_in:
- header
api_specs:
- filename: aws-app-mesh-openapi.yaml
  format: yaml
  label: AWS App Mesh API
  slug: aws-app-mesh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/openapi/aws-app-mesh-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws App Mesh Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS App Mesh secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/aws-app-mesh-openapi.yaml
  type: apiKey
slug: aws-app-mesh-authentication
source_filename: aws-app-mesh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-app-mesh-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/aws-app-mesh-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/authentication/aws-app-mesh-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
---
