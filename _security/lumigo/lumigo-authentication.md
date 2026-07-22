---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lumigo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumigo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lumigo
provider_slug: lumigo
scheme_count: 1
schemes:
- description: Lumigo access is managed through unique API tokens generated in the Lumigo platform under Settings. Tokens are passed as an x-api-key request header (used by the Lumigo API and the Copilot MCP server). Data is transmitted over HTTPS (TLS 1.2+).
  in: header
  name: apiToken
  parameter: x-api-key
  sources:
  - https://lumigo.readme.io/docs/copilot-for-code
  type: apiKey
slug: lumigo-authentication
source_filename: lumigo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://lumigo.io/security/ ; https://lumigo.readme.io/docs/copilot-for-code\ndocs: https://docs.lumigo.io/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: >-\n      Lumigo access is managed through unique API tokens generated in the Lumigo\n      platform under Settings. Tokens are passed as an x-api-key request header\n      (used by the Lumigo API and the Copilot MCP server). Data is transmitted\n      over HTTPS (TLS 1.2+).\n    sources:\n      - https://lumigo.readme.io/docs/copilot-for-code\nnotes: >-\n  No public OpenAPI specification was located, so this profile is documented\n  from the security and Copilot-MCP documentation rather than derived from a\n  spec. AWS account connection is separately handled via IAM role assumption\n  following AWS best practices.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumigo/refs/heads/main/authentication/lumigo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Observability
- Monitoring
- Serverless
- Distributed Tracing
- OpenTelemetry
- AWS Lambda
- Microservices
- Logs
---
