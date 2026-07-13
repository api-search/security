---
api_key_in:
- header
api_specs:
- filename: aws-api-gateway-v1-openapi.yml
  format: yaml
  label: Amazon API Gateway V1 (REST)
  slug: aws-api-gateway-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-v1-openapi.yml
- filename: aws-api-gateway-v2-openapi.yml
  format: yaml
  label: Amazon API Gateway V2 (HTTP and WebSocket)
  slug: aws-api-gateway-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-v2-openapi.yml
- filename: aws-api-gateway-management-openapi.yml
  format: yaml
  label: Amazon API Gateway Management API
  slug: aws-api-gateway-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-management-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Api Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon API Gateway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed request.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/aws-api-gateway-management-openapi.yml
  - openapi/aws-api-gateway-v1-openapi.yml
  - openapi/aws-api-gateway-v2-openapi.yml
  type: apiKey
slug: aws-api-gateway-authentication
source_filename: aws-api-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-api-gateway-management-openapi.yml, openapi/aws-api-gateway-v1-openapi.yml,\n  openapi/aws-api-gateway-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed request.\n  sources:\n  - openapi/aws-api-gateway-management-openapi.yml\n  - openapi/aws-api-gateway-v1-openapi.yml\n  - openapi/aws-api-gateway-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/authentication/aws-api-gateway-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Gateway
- Cloud
- REST
- HTTP
- WebSocket
- Serverless
- MCP
- AgentCore
- Developer Portal
---
