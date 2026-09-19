---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: monte-carlo-graph-ql-api-openapi.yml
  format: yaml
  label: Monte Carlo Graph QL API
  slug: monte-carlo-graph-ql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monte-carlo/refs/heads/main/openapi/monte-carlo-graph-ql-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Monte Carlo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monte Carlo secures its APIs with apiKey and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Monte Carlo
provider_slug: monte-carlo
scheme_count: 5
schemes:
- apis:
  - monte-carlo:graphql-api
  description: Personal or account-level API key (Key ID + Secret, 56-character base64 strings from 42 random bytes; the secret is shown once). Sent as `x-mcd-id` and `x-mcd-token` on every request. Created at Settings -> API with a chosen key type and expiration.
  in: header
  name: mcdHeaders
  paired_with: x-mcd-token
  parameter: x-mcd-id
  sources:
  - openapi/monte-carlo-graph-ql-api-openapi.yml
  - https://docs.getmontecarlo.com/docs/api-authentication
  type: apiKey
- apis:
  - monte-carlo:graphql-api
  description: Personal or Service OAuth clients exchange client ID + secret for a short-lived JWT sent as a Bearer token.
  flow: clientCredentials
  name: oauthClientCredentials
  scopes:
  - https://api.getmontecarlo.com/access
  - https://instance.getmontecarlo.com/{instance_id}
  sources:
  - https://docs.getmontecarlo.com/docs/api-authentication#authenticating-with-oauth-client-credentials
  token_url: https://api.getmontecarlo.com/oauth2/token
  type: oauth2
- apis:
  - monte-carlo:push-ingest-api
  description: Dedicated Ingestion-scoped integration key, optionally restricted to warehouse UUIDs; standard API keys are rejected and it cannot call GraphQL.
  in: header
  name: ingestionKey
  paired_with: x-mcd-token
  parameter: x-mcd-id
  sources:
  - https://docs.getmontecarlo.com/docs/push-ingest-api#authentication
  type: apiKey
- apis:
  - monte-carlo:mcp-server
  authorization_server: https://auth.getmontecarlo.com
  authorization_url: https://auth.getmontecarlo.com/oauth2/authorize
  dynamic_client_registration: true
  flow: authorizationCode
  name: mcpOAuth
  pkce: S256
  scopes:
  - offline_access
  sources:
  - https://docs.getmontecarlo.com/docs/mcp-server
  - https://auth.getmontecarlo.com/.well-known/oauth-authorization-server
  token_url: https://auth.getmontecarlo.com/oauth2/token
  type: oauth2
- apis:
  - monte-carlo:mcp-server
  description: MCP Server key type only (also accepted as x-mcd-id / x-mcd-token headers).
  format: <KEY_ID>:<KEY_SECRET>
  name: mcpServerKey
  scheme: bearer
  sources:
  - https://docs.getmontecarlo.com/docs/mcp-server#option-3-api-keys-advanced
  type: http
slug: monte-carlo-authentication
source_filename: monte-carlo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: https://docs.getmontecarlo.com/docs/api-authentication\ndocs: https://docs.getmontecarlo.com/docs/api-authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: mcdHeaders\n  type: apiKey\n  in: header\n  parameter: x-mcd-id\n  paired_with: x-mcd-token\n  apis: [monte-carlo:graphql-api]\n  description: >-\n    Personal or account-level API key (Key ID + Secret, 56-character base64 strings from 42 random bytes;\n    the secret is shown once). Sent as `x-mcd-id` and `x-mcd-token` on every request. Created at\n    Settings -> API with a chosen key type and expiration.\n  sources:\n  - openapi/monte-carlo-graph-ql-api-openapi.yml\n  - https://docs.getmontecarlo.com/docs/api-authentication\n- name: oauthClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  apis: [monte-carlo:graphql-api]\n  token_url: https://api.getmontecarlo.com/oauth2/token\n  scopes: ['https://api.getmontecarlo.com/access',\
  \ 'https://instance.getmontecarlo.com/{instance_id}']\n  description: Personal or Service OAuth clients exchange client ID + secret for a short-lived JWT sent as a Bearer token.\n  sources:\n  - https://docs.getmontecarlo.com/docs/api-authentication#authenticating-with-oauth-client-credentials\n- name: ingestionKey\n  type: apiKey\n  in: header\n  parameter: x-mcd-id\n  paired_with: x-mcd-token\n  apis: [monte-carlo:push-ingest-api]\n  description: Dedicated Ingestion-scoped integration key, optionally restricted to warehouse UUIDs; standard API keys are rejected and it cannot call GraphQL.\n  sources:\n  - https://docs.getmontecarlo.com/docs/push-ingest-api#authentication\n- name: mcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  dynamic_client_registration: true\n  apis: [monte-carlo:mcp-server]\n  authorization_server: https://auth.getmontecarlo.com\n  authorization_url: https://auth.getmontecarlo.com/oauth2/authorize\n  token_url: https://auth.getmontecarlo.com/oauth2/token\n\
  \  scopes: [offline_access]\n  sources:\n  - https://docs.getmontecarlo.com/docs/mcp-server\n  - https://auth.getmontecarlo.com/.well-known/oauth-authorization-server\n- name: mcpServerKey\n  type: http\n  scheme: bearer\n  format: '<KEY_ID>:<KEY_SECRET>'\n  apis: [monte-carlo:mcp-server]\n  description: MCP Server key type only (also accepted as x-mcd-id / x-mcd-token headers).\n  sources:\n  - https://docs.getmontecarlo.com/docs/mcp-server#option-3-api-keys-advanced\nsso: SSO and SCIM provisioning (Okta, Microsoft Entra ID) for the web app, Scale plan and above.\nkey_rotation: https://docs.getmontecarlo.com/docs/rotating-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monte-carlo/refs/heads/main/authentication/monte-carlo-authentication.yml
summary_line: apiKey/oauth2 · 5 schemes
tags:
- Data Observability
- Data Quality
- Data Reliability
- Data Lake
- Data Warehouse
- Lineage
- Monitoring
- AI Observability
---
