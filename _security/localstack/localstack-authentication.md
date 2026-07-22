---
api_key_in: []
api_specs:
- filename: localstack-openapi-original.yml
  format: yaml
  label: LocalStack REST API for Community
  slug: localstack-rest-api-for-community
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localstack/refs/heads/main/openapi/localstack-openapi-original.yml
auth_types:
- none
- auth-token
description: ''
kind: authentication
layout: security
method: searched
name: Localstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: LocalStack secures its APIs with none and auth-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LocalStack
provider_slug: localstack
scheme_count: 2
schemes:
- detail: Unauthenticated; no securitySchemes defined in the OpenAPI document.
  name: none
  scope: local REST API (openapi/localstack-openapi-original.yml)
  type: none
- detail: The Auth Token is supplied via the LOCALSTACK_AUTH_TOKEN environment variable to the container and to the MCP server (marked isRequired + isSecret in the MCP Server Card).
  docs: https://docs.localstack.cloud/aws/getting-started/auth-token/
  in: environment
  name: auth-token
  parameter: LOCALSTACK_AUTH_TOKEN
  scope: platform activation + MCP server + licensed features
  secret: true
  type: apiKey
slug: localstack-authentication
source_filename: localstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  openapi/localstack-openapi-original.yml, https://docs.localstack.cloud/,\n  https://docs.localstack.cloud/.well-known/mcp/server-card.json\nsummary:\n  types: [none, auth-token]\n  notes: >-\n    Two distinct surfaces. (1) The LocalStack REST API for Community (the local emulator control\n    plane at localhost.localstack.cloud:4566) declares NO securitySchemes and requires no\n    authentication — it is bound to the developer's own machine. (2) The LocalStack platform and\n    licensed (Pro/Ultimate/Enterprise) features are activated with a LocalStack Auth Token.\nschemes:\n  - name: none\n    type: none\n    scope: local REST API (openapi/localstack-openapi-original.yml)\n    detail: Unauthenticated; no securitySchemes defined in the OpenAPI document.\n  - name: auth-token\n    type: apiKey\n    in: environment\n    parameter: LOCALSTACK_AUTH_TOKEN\n    scope: platform activation + MCP server + licensed features\n \
  \   secret: true\n    docs: https://docs.localstack.cloud/aws/getting-started/auth-token/\n    detail: >-\n      The Auth Token is supplied via the LOCALSTACK_AUTH_TOKEN environment variable to the\n      container and to the MCP server (marked isRequired + isSecret in the MCP Server Card).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localstack/refs/heads/main/authentication/localstack-authentication.yml
summary_line: none/auth-token · 2 schemes
tags:
- Company
- Developer Tools
- Cloud
- Emulator
- Testing
- DevOps
- Serverless
- Infrastructure
---
