---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Stack Machine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stack Machine secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stack Machine
provider_slug: stack-machine
scheme_count: 1
schemes:
- description: A StackMachine API key exported from the dashboard (or a demo key for local experiments), supplied to the SDK via the STACKMACHINE_API_KEY environment variable and sent by the client transport on every GraphQL request.
  env_var: STACKMACHINE_API_KEY
  in: header
  key_management:
    dashboard: https://dashboard.stackmachine.com/
    graphql_mutations:
    - generateApiToken
    - rotateApiKey
    - updateApiKey
    - createNamespaceApiKey
    - deleteNamespaceApiKey
    - revokeApiToken
  name: apiKey
  type: apiKey
slug: stack-machine-authentication
source_filename: stack-machine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.stackmachine.com/getting-started/installation\ndocs: https://docs.stackmachine.com/getting-started/client\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  transport: GraphQL over HTTPS (POST https://api.stackmachine.com/graphql)\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: A StackMachine API key exported from the dashboard (or a demo key for\n    local experiments), supplied to the SDK via the STACKMACHINE_API_KEY environment\n    variable and sent by the client transport on every GraphQL request.\n  env_var: STACKMACHINE_API_KEY\n  key_management:\n    dashboard: https://dashboard.stackmachine.com/\n    graphql_mutations:\n    - generateApiToken\n    - rotateApiKey\n    - updateApiKey\n    - createNamespaceApiKey\n    - deleteNamespaceApiKey\n    - revokeApiToken\nnotes: The GraphQL schema also exposes token-based session flows (tokenAuth, socialAuth,\n  refreshAccessToken,\
  \ verifyAccessToken, revokeAccessToken) used by the dashboard;\n  programmatic SDK access is via the API key above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-machine/refs/heads/main/authentication/stack-machine-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Infrastructure
- Serverless
- WebAssembly
- Edge Compute
- AI Applications
- GraphQL
- Platform as a Service
- Deployment
- Hosting
- DNS
- Databases
---
