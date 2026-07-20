---
api_key_in: []
api_specs:
- filename: notion-openapi.yml
  format: yaml
  label: Notion API
  slug: notion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/openapi/notion-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Notion Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Notion secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Notion
provider_slug: notion
scheme_count: 2
schemes:
- description: Notion API uses bearer token authentication. Obtain an integration token from https://www.notion.so/my-integrations. Pass the token in the Authorization header as "Bearer {token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/notion-openapi.yml
  token_types:
  - internal integration token
  - personal access token
  type: http
- capabilities_docs: https://developers.notion.com/reference/capabilities
  description: Public connections authorize end users via OAuth 2.0 authorization code flow. What a token can do is governed by integration "capabilities" (read/insert/update content, read/insert comments, read user info) rather than granular OAuth scopes.
  docs: https://developers.notion.com/guides/get-started/authorization
  flows:
  - authorizationUrl: https://api.notion.com/v1/oauth/authorize
    flow: authorizationCode
    refresh: true
    tokenUrl: https://api.notion.com/v1/oauth/token
  name: oauth2
  sources:
  - https://developers.notion.com/reference/authentication
  type: oauth2
slug: notion-authentication
source_filename: notion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/notion-openapi.yml\ndocs: https://developers.notion.com/reference/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  authorization_model: capabilities\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Notion API uses bearer token authentication. Obtain an integration token from\n    https://www.notion.so/my-integrations. Pass the token in the Authorization header as \"Bearer\n    {token}\".\n  token_types:\n  - internal integration token\n  - personal access token\n  sources:\n  - openapi/notion-openapi.yml\n- name: oauth2\n  type: oauth2\n  description: >-\n    Public connections authorize end users via OAuth 2.0 authorization code flow.\n    What a token can do is governed by integration \"capabilities\" (read/insert/update\n    content, read/insert comments, read user info) rather than granular OAuth scopes.\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://api.notion.com/v1/oauth/authorize\n    tokenUrl: https://api.notion.com/v1/oauth/token\n    refresh: true\n  docs: https://developers.notion.com/guides/get-started/authorization\n  capabilities_docs: https://developers.notion.com/reference/capabilities\n  sources:\n  - https://developers.notion.com/reference/authentication\nnotes:\n  - The remote Notion MCP server (mcp.notion.com) requires user-based OAuth; discovery at /.well-known/oauth-authorization-server.\n  - No granular OAuth scope surface — capabilities are configured per integration; scopes/ artifact intentionally omitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/authentication/notion-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Collaboration
- Database
- Ideas
- Notes
- Productivity
- Projects
- T1
- Tasks
- Wiki
- Workspace
---
