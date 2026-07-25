---
api_key_in:
- header
api_specs:
- filename: aws-api-gateway-apikeys-api-openapi.yml
  format: yaml
  label: Amazon API Gateway ApiKeys API
  slug: aws-api-gateway-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-apikeys-api-openapi.yml
- filename: aws-api-gateway-apis-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Apis API
  slug: aws-api-gateway-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-apis-api-openapi.yml
- filename: aws-api-gateway-authorizers-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Authorizers API
  slug: aws-api-gateway-authorizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-authorizers-api-openapi.yml
- filename: aws-api-gateway-connections-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Connections API
  slug: aws-api-gateway-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-connections-api-openapi.yml
- filename: aws-api-gateway-deployments-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Deployments API
  slug: aws-api-gateway-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-deployments-api-openapi.yml
- filename: aws-api-gateway-integrations-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Integrations API
  slug: aws-api-gateway-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-integrations-api-openapi.yml
- filename: aws-api-gateway-methods-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Methods API
  slug: aws-api-gateway-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-methods-api-openapi.yml
- filename: aws-api-gateway-resources-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Resources API
  slug: aws-api-gateway-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-resources-api-openapi.yml
- filename: aws-api-gateway-restapis-api-openapi.yml
  format: yaml
  label: Amazon API Gateway RestApis API
  slug: aws-api-gateway-restapis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-restapis-api-openapi.yml
- filename: aws-api-gateway-routes-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Routes API
  slug: aws-api-gateway-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-routes-api-openapi.yml
- filename: aws-api-gateway-stages-api-openapi.yml
  format: yaml
  label: Amazon API Gateway Stages API
  slug: aws-api-gateway-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-stages-api-openapi.yml
- filename: aws-api-gateway-usageplans-api-openapi.yml
  format: yaml
  label: Amazon API Gateway UsagePlans API
  slug: aws-api-gateway-usageplans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/openapi/aws-api-gateway-usageplans-api-openapi.yml
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
