---
api_key_in: []
api_specs:
- filename: external-v1-openapi-original.yml
  format: yaml
  label: WorkBoard External API v1
  slug: workboard-external-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/external-v1-openapi-original.yml
- filename: public-v2-openapi-original.yml
  format: yaml
  label: WorkBoard Public API v2
  slug: workboard-public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/public-v2-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Workboard Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: WorkBoard secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: WorkBoard
provider_slug: workboard
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT Authorization header using the Bearer scheme. All v1 and v2 requests require it.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/external-v1-openapi-original.yml
  - openapi/public-v2-openapi-original.yml
  type: http
- description: OAuth 2.0 documented on the developer portal (not declared in the OpenAPI). Recommended for multi-user applications; apps are registered in WorkBoard at Settings -> Custom Integrations. The access_token is valid for one year and can be revoked.
  flows:
  - authorizationUrl: https://www.myworkboard.com/wb/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://www.myworkboard.com/wb/oauth/revoke/
    tokenUrl: https://www.myworkboard.com/wb/oauth/token
  name: oauth2
  sources:
  - https://www.workboard.com/developer
  type: oauth2
slug: workboard-authentication
source_filename: workboard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/external-v1-openapi-original.yml, openapi/public-v2-openapi-original.yml\ndocs: https://www.workboard.com/developer\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Authorization header using the Bearer scheme. All v1 and v2 requests require it.\n  sources:\n  - openapi/external-v1-openapi-original.yml\n  - openapi/public-v2-openapi-original.yml\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 documented on the developer portal (not declared in the\n    OpenAPI). Recommended for multi-user applications; apps are registered\n    in WorkBoard at Settings -> Custom Integrations. The access_token is\n    valid for one year and can be revoked.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.myworkboard.com/wb/oauth/authorize\n    tokenUrl: https://www.myworkboard.com/wb/oauth/token\n\
  \    revocationUrl: https://www.myworkboard.com/wb/oauth/revoke/\n  sources:\n  - https://www.workboard.com/developer\ntoken_types:\n  - name: instant token\n    description: Single-click token generation for testing or single-user apps (Settings -> Custom Integrations, https://www.myworkboard.com/wb/user/profile/edit?do=mgApp).\n  - name: OAuth 2.0 access token\n    description: Browser-based authorization code flow; token valid one year, revocable.\n  - name: SCIM token\n    description: Admin-requested bearer token for the SCIM 2.0 provisioning API (https://myworkboard.com/wb/apis/scim).\n  - name: MCP personal access token\n    description: Generated in Settings -> Custom Integrations -> App tab; shown once; only valid for the MCP server, not other WorkBoard APIs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/authentication/workboard-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- OKRs
- Strategy Execution
- Goals
- Key Results
- Enterprise
- AI Agents
- Performance Management
- Strategic Portfolio Management
---
