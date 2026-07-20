---
api_key_in: []
api_specs:
- filename: coda-project-openapi-original.json
  format: json
  label: Coda Docs API
  slug: coda-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda-project/refs/heads/main/openapi/coda-project-openapi-original.json
- filename: coda-project-admin-openapi-original.json
  format: json
  label: Coda Admin API
  slug: coda-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda-project/refs/heads/main/openapi/coda-project-admin-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Coda Project Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coda Project secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coda Project
provider_slug: coda-project
scheme_count: 2
schemes:
- bearerFormat: UUID
  description: 'The Superhuman Docs Admin API can be accessed using an API token, which can be obtained from [*My account*](https://docs.superhuman.com/account)

    in Superhuman Docs. This token should be specified by setting a header as follows.


    ```Authorization: Bearer <api_token>```


    Keep your token safe, as anyone who gets access to it can access your account. Once a token is created

    it cannot be viewed or modi'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/coda-project-admin-openapi-original.json
  - openapi/coda-project-openapi-original.json
  type: http
- flows:
    authorizationCode:
      authorizationUrl: https://coda.io/v4/api/oauth2/authorize
      registrationUrl: https://coda.io/v4/api/oauth2/register
      scopes:
        mcp:all: Full read/write access via the remote MCP server.
      tokenUrl: https://coda.io/v4/api/oauth2/token
  name: OAuth2
  note: Separate OAuth 2.0 authorization server powering third-party apps and the official remote MCP server. PKCE (S256), dynamic client registration, authorization_code grant, scope mcp:all.
  source: well-known/coda-project-oauth-authorization-server.json
  type: oauth2
slug: coda-project-authentication
source_filename: coda-project-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/coda-project-admin-openapi-original.json, openapi/coda-project-openapi-original.json, https://coda.io/.well-known/oauth-authorization-server\ndocs: https://coda.io/developers/apis/v1#section/Authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  token_restrictions: >-\n    Docs API bearer tokens can be created with restrictions limiting them to read, write, or\n    read+write access, and scoped to specific documents or tables. /whoami and\n    /resolveBrowserLink are special-cased.\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: UUID\n  description: |-\n    The Superhuman Docs Admin API can be accessed using an API token, which can be obtained from [*My account*](https://docs.superhuman.com/account)\n    in Superhuman Docs. This token should be specified by setting a header as follows.\n\n    ```Authorization: Bearer <api_token>```\n\n    Keep your\
  \ token safe, as anyone who gets access to it can access your account. Once a token is created\n    it cannot be viewed or modi\n  sources:\n  - openapi/coda-project-admin-openapi-original.json\n  - openapi/coda-project-openapi-original.json\n- name: OAuth2\n  type: oauth2\n  source: well-known/coda-project-oauth-authorization-server.json\n  note: >-\n    Separate OAuth 2.0 authorization server powering third-party apps and the official remote\n    MCP server. PKCE (S256), dynamic client registration, authorization_code grant, scope mcp:all.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://coda.io/v4/api/oauth2/authorize\n      tokenUrl: https://coda.io/v4/api/oauth2/token\n      registrationUrl: https://coda.io/v4/api/oauth2/register\n      scopes:\n        \"mcp:all\": Full read/write access via the remote MCP server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coda-project/refs/heads/main/authentication/coda-project-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Productivity
- Documents
- Spreadsheets
- Collaboration
- No-Code
- Workspace
- AI
- Content Management
- SaaS
---
