---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AgentSQL Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentSQL declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentSQL
provider_slug: agentsql-cn
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'Agent API Key provided per Agent, used as Bearer token in Authorization header. Example: Authorization: Bearer <Agent API Key>'
  scheme: bearer
  type: http
slug: agentsql-cn-authentication
source_filename: agentsql-cn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://agentsql.cn/assets/docs/agentsql-getting-started-v4.3.0.pdf\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: API Key\n    description: \"Agent API Key provided per Agent, used as Bearer token in Authorization header. Example: Authorization: Bearer <Agent API Key>\"\n"
source_yaml_url: https://artifacts.apis.io/agentsql-cn/authentication/agentsql-cn-authentication.yml
summary_line: 1 scheme
tags:
- Database
- Security
- Artificial Intelligence
- Open Source
- Gateways
---
