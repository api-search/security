---
anonymous_access: false
api_key_in: []
api_specs:
- filename: worklittle-job-boards-api-openapi.yml
  format: yaml
  label: Worklittle Job Boards API
  slug: worklittle-job-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/openapi/worklittle-job-boards-api-openapi.yml
- filename: worklittle-jobs-api-openapi.yml
  format: yaml
  label: Worklittle Jobs API
  slug: worklittle-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/openapi/worklittle-jobs-api-openapi.yml
- filename: worklittle-platform-api-openapi.yml
  format: yaml
  label: Worklittle Business Platform API
  slug: worklittle-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/openapi/worklittle-platform-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Worklittle Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Worklittle secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Worklittle
provider_slug: worklittle
scheme_count: 2
schemes:
- bearerFormat: sk-wl-api01
  description: API keys created in Worklittle Business (worklittle.com/business/api-keys), prefix sk-wl-api01-, shown once. Sent as Authorization Bearer on REST, MCP and CLI/SDK (WORKLITTLE_API_KEY). Keys carry scopes (jobs:read, jobs:apply, jobs:post, jobs:applications, webhooks:manage, agent:tools) and inherit the creator's role. Default 60 requests/minute per key. Public job-board GETs and applies work without a key under IP rate limits.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/worklittle-jobs-api-openapi.yml
  - openapi/worklittle-platform-api-openapi.yml
  type: http
- description: 'OAuth 2.0 authorization server on api.worklittle.com (RFC 8414 metadata saved at well-known/worklittle-oauth-authorization-server.json) used by MCP Connect sessions: authorization_code + refresh_token, PKCE S256, dynamic client registration (RFC 7591), client_id metadata documents and resource indicators. The MCP server publishes a matching RFC 9728 protected-resource document naming this issuer.'
  flows:
  - authorizationUrl: https://api.worklittle.com/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.worklittle.com/oauth/token
  name: mcpConnectOAuth
  sources:
  - well-known/worklittle-oauth-authorization-server.json
  type: oauth2
slug: worklittle-authentication
source_filename: worklittle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/worklittle-jobs-api-openapi.yml, openapi/worklittle-platform-api-openapi.yml\ndocs: https://docs.worklittle.com/jobs/get-started/api-keys\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk-wl-api01\n  description: >-\n    API keys created in Worklittle Business (worklittle.com/business/api-keys), prefix sk-wl-api01-,\n    shown once. Sent as Authorization Bearer on REST, MCP and CLI/SDK (WORKLITTLE_API_KEY). Keys\n    carry scopes (jobs:read, jobs:apply, jobs:post, jobs:applications, webhooks:manage, agent:tools)\n    and inherit the creator's role. Default 60 requests/minute per key. Public job-board GETs and\n    applies work without a key under IP rate limits.\n  sources:\n  - openapi/worklittle-jobs-api-openapi.yml\n  - openapi/worklittle-platform-api-openapi.yml\n- name: mcpConnectOAuth\n  type: oauth2\n\
  \  description: >-\n    OAuth 2.0 authorization server on api.worklittle.com (RFC 8414 metadata saved at\n    well-known/worklittle-oauth-authorization-server.json) used by MCP Connect sessions:\n    authorization_code + refresh_token, PKCE S256, dynamic client registration (RFC 7591),\n    client_id metadata documents and resource indicators. The MCP server publishes a matching\n    RFC 9728 protected-resource document naming this issuer.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.worklittle.com/oauth/authorize\n    tokenUrl: https://api.worklittle.com/oauth/token\n    scopes: 6\n  sources:\n  - well-known/worklittle-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/authentication/worklittle-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Job Search
- ATS
- Recruiting
- Workforce Intelligence
- Job Boards
- Webhooks
- MCP
---
