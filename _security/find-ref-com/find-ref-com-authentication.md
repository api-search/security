---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'find-ref exposes only an MCP endpoint (https://api.find-ref.com/mcp) protected by

  OAuth 2.0. The authorization server metadata at

  https://api.find-ref.com/.well-known/oauth-authorization-server lists the

  authorization_code and refresh_token grant types, PKCE with S256, dynamic client

  registration, and the scopes findref.read + offline_access.

  '
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Find Ref Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: find-ref declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: find-ref
provider_slug: find-ref-com
scheme_count: 1
schemes:
- dynamic_client_registration:
    endpoint: https://api.find-ref.com/mcp/register
    supported: true
  flows:
    authorizationCode:
      authorizationUrl: https://api.find-ref.com/mcp/authorize
      refreshUrl: https://api.find-ref.com/mcp/token
      scopes:
        findref.read: Read-only access to find-ref evidence search (search, original-text lookup, citation cross-check).
        offline_access: Issue a refresh_token so the client can refresh the access_token without re-prompting.
      tokenUrl: https://api.find-ref.com/mcp/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.find-ref.com
  name: oauth2
  pkce:
    methods:
    - S256
    required: true
  protected_resources:
  - https://api.find-ref.com/mcp
  response_types:
  - code
  revocation_endpoint: https://api.find-ref.com/mcp/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: find-ref-com-authentication
source_filename: find-ref-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://api.find-ref.com/.well-known/oauth-authorization-server\nname: find-ref authentication\ndescription: |\n  find-ref exposes only an MCP endpoint (https://api.find-ref.com/mcp) protected by\n  OAuth 2.0. The authorization server metadata at\n  https://api.find-ref.com/.well-known/oauth-authorization-server lists the\n  authorization_code and refresh_token grant types, PKCE with S256, dynamic client\n  registration, and the scopes findref.read + offline_access.\nschemes:\n  - type: oauth2\n    name: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://api.find-ref.com/mcp/authorize\n        tokenUrl: https://api.find-ref.com/mcp/token\n        refreshUrl: https://api.find-ref.com/mcp/token\n        scopes:\n          findref.read: Read-only access to find-ref evidence search (search, original-text lookup, citation cross-check).\n          offline_access: Issue a refresh_token so the client can\
  \ refresh the access_token without re-prompting.\n    pkce:\n      required: true\n      methods:\n        - S256\n    dynamic_client_registration:\n      supported: true\n      endpoint: https://api.find-ref.com/mcp/register\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - none\n    response_types:\n      - code\n    grant_types:\n      - authorization_code\n      - refresh_token\n    revocation_endpoint: https://api.find-ref.com/mcp/token\n    issuer: https://api.find-ref.com\n    protected_resources:\n      - https://api.find-ref.com/mcp\nevidence:\n  - url: https://api.find-ref.com/.well-known/oauth-authorization-server\n    status: 200\n    fetched: '2026-11-07'\n  - url: https://find-ref.com/connect/\n    status: 200\n    fetched: '2026-11-07'\n"
source_yaml_url: https://artifacts.apis.io/find-ref-com/authentication/find-ref-com-authentication.yml
summary_line: 1 scheme
tags:
- Accounting
- Tax
- Legal Research
- Labor Law
- AI Assistant
- MCP
- Korea
- Reference Search
---
