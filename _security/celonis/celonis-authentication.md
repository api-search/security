---
api_key_in:
- header
api_specs:
- filename: celonis-knowledge-model-openapi.yaml
  format: yaml
  label: Celonis Knowledge Model API
  slug: celonis-knowledge-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-knowledge-model-openapi.yaml
- filename: celonis-agents-ai-openapi.yaml
  format: yaml
  label: Celonis AI Agent API
  slug: celonis-ai-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-agents-ai-openapi.yaml
- filename: celonis-subscription-openapi.yaml
  format: yaml
  label: Celonis Event Subscription API
  slug: celonis-event-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-subscription-openapi.yaml
- filename: celonis-mlwb-openapi.yaml
  format: yaml
  label: Celonis Machine Learning Workbench API
  slug: celonis-machine-learning-workbench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-mlwb-openapi.yaml
- filename: celonis-team-openapi.yaml
  format: yaml
  label: Celonis Team API
  slug: celonis-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-team-openapi.yaml
- filename: celonis-permissions-openapi.yaml
  format: yaml
  label: Celonis Permissions API
  slug: celonis-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-permissions-openapi.yaml
- filename: celonis-mcp-tool-calling-openapi.yaml
  format: yaml
  label: Celonis Agent Tools (MCP) Tool Calling API
  slug: celonis-agent-tools-mcp-tool-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-mcp-tool-calling-openapi.yaml
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Celonis Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Celonis secures its APIs with oauth2, http, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Celonis
provider_slug: celonis
scheme_count: 4
schemes:
- client_auth:
  - client_secret_basic
  - client_secret_post
  flows:
  - flow: clientCredentials
    tokenUrl: https://{team_domain}.{realm}.celonis.cloud/oauth2/token
  - authorizationUrl: https://{team_domain}.{realm}.celonis.cloud/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://{team_domain}.{realm}.celonis.cloud/oauth2/token
  name: OAuth2
  source: https://developer.celonis.com/celonis-apis/oauth-authentication/
  token_lifetime_seconds: 899
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/celonis-agents-ai-openapi.yaml
  - openapi/celonis-knowledge-model-openapi.yaml
  - openapi/celonis-subscription-openapi.yaml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: AppKey
  sources:
  - openapi/celonis-agents-ai-openapi.yaml
  - openapi/celonis-knowledge-model-openapi.yaml
  - openapi/celonis-subscription-openapi.yaml
  status: deprecating
  type: apiKey
- description: Prefix the token with "AppKey " or "Bearer " to indicate the authorization type.
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/celonis-permissions-openapi.yaml
  - openapi/celonis-team-openapi.yaml
  type: apiKey
slug: celonis-authentication
source_filename: celonis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/*.yaml + https://developer.celonis.com/celonis-apis/auth/\ndocs: https://developer.celonis.com/celonis-apis/auth/\noauth_docs: https://developer.celonis.com/celonis-apis/oauth-authentication/\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  recommended: oauth2\n  deprecating:\n  - User API Key (Bearer)\n  - Application API Key (AppKey)\nnotes: >-\n  Celonis Platform APIs authenticate via the Authorization header. OAuth 2.0 is the\n  recommended method (User API Key and Application API Key are deprecating). OAuth\n  access tokens are short-lived (~899s / 15 min) and support refresh; client secrets\n  can be rotated. Client-credentials (machine-to-machine) and authorization-code\n  (user delegation) grants are supported, with client_secret_basic and\n  client_secret_post client authentication. Base host is\n  https://{team_domain}.{realm}.celonis.cloud;\
  \ token endpoint is\n  https://{team_domain}.{realm}.celonis.cloud/oauth2/token.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{team_domain}.{realm}.celonis.cloud/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://{team_domain}.{realm}.celonis.cloud/oauth2/authorize\n    tokenUrl: https://{team_domain}.{realm}.celonis.cloud/oauth2/token\n  token_lifetime_seconds: 899\n  client_auth: [client_secret_basic, client_secret_post]\n  source: https://developer.celonis.com/celonis-apis/oauth-authentication/\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/celonis-agents-ai-openapi.yaml\n  - openapi/celonis-knowledge-model-openapi.yaml\n  - openapi/celonis-subscription-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: AppKey\n  status: deprecating\n  sources:\n  - openapi/celonis-agents-ai-openapi.yaml\n  - openapi/celonis-knowledge-model-openapi.yaml\n\
  \  - openapi/celonis-subscription-openapi.yaml\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Prefix the token with \"AppKey \" or \"Bearer \" to indicate the authorization type.\n  sources:\n  - openapi/celonis-permissions-openapi.yaml\n  - openapi/celonis-team-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/authentication/celonis-authentication.yml
summary_line: oauth2/http/apiKey · 4 schemes
tags:
- Company
- Automation
- Process Mining
- Process Intelligence
- Data
- Analytics
- Machine Learning
- AI Agents
- Enterprise
---
