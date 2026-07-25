---
api_key_in:
- header
api_specs:
- filename: celonis-agents-conversation-api-openapi.yml
  format: yaml
  label: Celonis Agents - Conversation API
  slug: celonis-agents-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-agents-conversation-api-openapi.yml
- filename: celonis-beta-odata-protocol-api-openapi.yml
  format: yaml
  label: 'Celonis Beta: OData Protocol API'
  slug: celonis-beta-odata-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-beta-odata-protocol-api-openapi.yml
- filename: celonis-beta-semantics-for-3p-ai-agents-api-openapi.yml
  format: yaml
  label: 'Celonis Beta: Semantics for 3P AI Agents API'
  slug: celonis-beta-semantics-for-3p-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-beta-semantics-for-3p-ai-agents-api-openapi.yml
- filename: celonis-data-api-openapi.yml
  format: yaml
  label: Celonis Data API
  slug: celonis-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-data-api-openapi.yml
- filename: celonis-job-execution-api-openapi.yml
  format: yaml
  label: Celonis Job Execution API
  slug: celonis-job-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-job-execution-api-openapi.yml
- filename: celonis-job-execution-group-api-openapi.yml
  format: yaml
  label: Celonis Job Execution Group API
  slug: celonis-job-execution-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-job-execution-group-api-openapi.yml
- filename: celonis-login-history-api-api-openapi.yml
  format: yaml
  label: Celonis Login History API API
  slug: celonis-login-history-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-login-history-api-api-openapi.yml
- filename: celonis-members-api-api-openapi.yml
  format: yaml
  label: Celonis Members API API
  slug: celonis-members-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-members-api-api-openapi.yml
- filename: celonis-notebook-api-openapi.yml
  format: yaml
  label: Celonis Notebook API
  slug: celonis-notebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-notebook-api-openapi.yml
- filename: celonis-notebook-execution-api-openapi.yml
  format: yaml
  label: Celonis Notebook Execution API
  slug: celonis-notebook-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-notebook-execution-api-openapi.yml
- filename: celonis-notebook-resources-api-openapi.yml
  format: yaml
  label: Celonis Notebook Resources API
  slug: celonis-notebook-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-notebook-resources-api-openapi.yml
- filename: celonis-openapi-tool-calling-api-openapi.yml
  format: yaml
  label: Celonis OpenAPI Tool Calling API
  slug: celonis-openapi-tool-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-openapi-tool-calling-api-openapi.yml
- filename: celonis-permissions-export-api-api-openapi.yml
  format: yaml
  label: Celonis Permissions Export API API
  slug: celonis-permissions-export-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-permissions-export-api-api-openapi.yml
- filename: celonis-schedule-api-openapi.yml
  format: yaml
  label: Celonis Schedule API
  slug: celonis-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-schedule-api-openapi.yml
- filename: celonis-schema-api-openapi.yml
  format: yaml
  label: Celonis Schema API
  slug: celonis-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-schema-api-openapi.yml
- filename: celonis-subscriptions-api-openapi.yml
  format: yaml
  label: Celonis Subscriptions API
  slug: celonis-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-subscriptions-api-openapi.yml
- filename: celonis-triggers-api-openapi.yml
  format: yaml
  label: Celonis Triggers API
  slug: celonis-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-triggers-api-openapi.yml
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
