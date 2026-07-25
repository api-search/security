---
api_key_in:
- header
api_specs:
- filename: amazon-api-gateway-websocket-asyncapi.yml
  format: yaml
  label: Amazon API Gateway WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/asyncapi/amazon-api-gateway-websocket-asyncapi.yml
- filename: amazon-api-gateway-api-keys-api-openapi.yml
  format: yaml
  label: Amazon API Gateway API Keys API
  slug: amazon-api-gateway-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-api-keys-api-openapi.yml
- filename: amazon-api-gateway-authorizers-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Authorizers API
  slug: amazon-api-gateway-authorizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-authorizers-api-openapi.yml
- filename: amazon-api-gateway-base-path-mappings-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Base Path Mappings API
  slug: amazon-api-gateway-base-path-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-base-path-mappings-api-openapi.yml
- filename: amazon-api-gateway-deployments-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Deployments API
  slug: amazon-api-gateway-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-deployments-api-openapi.yml
- filename: amazon-api-gateway-documentation-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Documentation API
  slug: amazon-api-gateway-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-documentation-api-openapi.yml
- filename: amazon-api-gateway-domain-names-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Domain Names API
  slug: amazon-api-gateway-domain-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-domain-names-api-openapi.yml
- filename: amazon-api-gateway-gateway-responses-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Gateway Responses API
  slug: amazon-api-gateway-gateway-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-gateway-responses-api-openapi.yml
- filename: amazon-api-gateway-methods-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Methods API
  slug: amazon-api-gateway-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-methods-api-openapi.yml
- filename: amazon-api-gateway-models-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Models API
  slug: amazon-api-gateway-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-models-api-openapi.yml
- filename: amazon-api-gateway-request-validators-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Request Validators API
  slug: amazon-api-gateway-request-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-request-validators-api-openapi.yml
- filename: amazon-api-gateway-resources-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Resources API
  slug: amazon-api-gateway-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-resources-api-openapi.yml
- filename: amazon-api-gateway-rest-apis-api-openapi.yml
  format: yaml
  label: Amazon API Gateway REST APIs API
  slug: amazon-api-gateway-rest-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-rest-apis-api-openapi.yml
- filename: amazon-api-gateway-stages-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Stages API
  slug: amazon-api-gateway-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-stages-api-openapi.yml
- filename: amazon-api-gateway-usage-plans-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Usage Plans API
  slug: amazon-api-gateway-usage-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-usage-plans-api-openapi.yml
- filename: amazon-api-gateway-vpc-links-api-openapi.yml
  format: yaml
  label: Amazon API Gateway VPC Links API
  slug: amazon-api-gateway-vpc-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/openapi/amazon-api-gateway-vpc-links-api-openapi.yml
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
