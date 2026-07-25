---
api_key_in:
- header
api_specs:
- filename: convex-asyncapi.yml
  format: yaml
  label: Convex Sync Protocol
  slug: sync-protocol
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/asyncapi/convex-asyncapi.yml
- filename: convex-accesstokens-api-openapi.yml
  format: yaml
  label: Convex AccessTokens API
  slug: convex-accesstokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-accesstokens-api-openapi.yml
- filename: convex-actions-api-openapi.yml
  format: yaml
  label: Convex Actions API
  slug: convex-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-actions-api-openapi.yml
- filename: convex-customdomains-api-openapi.yml
  format: yaml
  label: Convex CustomDomains API
  slug: convex-customdomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-customdomains-api-openapi.yml
- filename: convex-deploykeys-api-openapi.yml
  format: yaml
  label: Convex DeployKeys API
  slug: convex-deploykeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-deploykeys-api-openapi.yml
- filename: convex-deployments-api-openapi.yml
  format: yaml
  label: Convex Deployments API
  slug: convex-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-deployments-api-openapi.yml
- filename: convex-environmentvariables-api-openapi.yml
  format: yaml
  label: Convex EnvironmentVariables API
  slug: convex-environmentvariables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-environmentvariables-api-openapi.yml
- filename: convex-functions-api-openapi.yml
  format: yaml
  label: Convex Functions API
  slug: convex-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-functions-api-openapi.yml
- filename: convex-mutations-api-openapi.yml
  format: yaml
  label: Convex Mutations API
  slug: convex-mutations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-mutations-api-openapi.yml
- filename: convex-projects-api-openapi.yml
  format: yaml
  label: Convex Projects API
  slug: convex-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-projects-api-openapi.yml
- filename: convex-queries-api-openapi.yml
  format: yaml
  label: Convex Queries API
  slug: convex-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-queries-api-openapi.yml
- filename: convex-teams-api-openapi.yml
  format: yaml
  label: Convex Teams API
  slug: convex-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/openapi/convex-teams-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Convex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convex secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Convex
provider_slug: convex
scheme_count: 2
schemes:
- description: 'Authorization header using a deployment key, Team Access Token, or OAuth Application Token. The token must be prefixed with the string "Convex " (e.g. "Authorization: Convex prod:abc123..."). Deployment keys are created in the dashboard or via the Management API.'
  in: header
  name: convexAuth
  parameter: Authorization
  sources:
  - openapi/convex-deployment-platform-api-openapi.yml
  - openapi/convex-http-api-openapi.yml
  type: apiKey
- description: Bearer token from the application's configured authentication provider (e.g. Auth0, Clerk). Used for user-level authorization of function calls.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/convex-http-api-openapi.yml
  - openapi/convex-management-api-openapi.yml
  type: http
slug: convex-authentication
source_filename: convex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/convex-deployment-platform-api-openapi.yml, openapi/convex-http-api-openapi.yml,\n  openapi/convex-management-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: convexAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Authorization header using a deployment key, Team Access Token, or OAuth Application\n    Token. The token must be prefixed with the string \"Convex \" (e.g. \"Authorization: Convex\n    prod:abc123...\"). Deployment keys are created in the dashboard or via the Management API.'\n  sources:\n  - openapi/convex-deployment-platform-api-openapi.yml\n  - openapi/convex-http-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token from the application's configured authentication provider (e.g.\n    Auth0, Clerk). Used for user-level authorization of function calls.\n  sources:\n  - openapi/convex-http-api-openapi.yml\n\
  \  - openapi/convex-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/authentication/convex-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Backend
- Database
- Functions
- Real-Time
- Reactive
- Serverless
- TypeScript
---
