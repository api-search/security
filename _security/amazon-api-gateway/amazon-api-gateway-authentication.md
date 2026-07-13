---
api_key_in:
- header
api_specs:
- filename: API_Operations.html
  format: yaml
  label: Amazon API Gateway REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html
- filename: amazon-api-gateway-websocket-asyncapi.yml
  format: yaml
  label: Amazon API Gateway WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/asyncapi/amazon-api-gateway-websocket-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Api Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon API Gateway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-api-gateway-openapi.yaml
  - openapi/amazon-api-gateway-rest-openapi.yml
  type: apiKey
slug: amazon-api-gateway-authentication
source_filename: amazon-api-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-api-gateway-openapi.yaml, openapi/amazon-api-gateway-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-api-gateway-openapi.yaml\n  - openapi/amazon-api-gateway-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/authentication/amazon-api-gateway-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
---
