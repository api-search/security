---
api_key_in:
- cookie
api_specs:
- filename: prismatic-graphql-api-openapi.yml
  format: yaml
  label: Prismatics GraphQL API
  slug: prismatics-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/openapi/prismatic-graphql-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Prismatic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prismatic secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Prismatic
provider_slug: prismatic
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token obtained via the Prismatic web app, CLI tool (me:token subcommand), or the /auth/refresh endpoint. Pass as Authorization Bearer header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/prismatic-graphql-api-openapi.yml
  type: http
- description: Session cookie from Prismatic web application login
  in: cookie
  name: cookieAuth
  parameter: session
  sources:
  - openapi/prismatic-graphql-api-openapi.yml
  type: apiKey
slug: prismatic-authentication
source_filename: prismatic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prismatic-graphql-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained via the Prismatic web app, CLI tool (me:token subcommand),\n    or the /auth/refresh endpoint. Pass as Authorization Bearer header.\n  sources:\n  - openapi/prismatic-graphql-api-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: Session cookie from Prismatic web application login\n  sources:\n  - openapi/prismatic-graphql-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/authentication/prismatic-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Embedded iPaaS
- Integrations
- Workflows
- Connectors
- AI Agents
- MCP
- Code-Native
- Low-Code
---
