---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Filedone Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: filedone declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: filedone
provider_slug: filedone-ai
scheme_count: 2
schemes:
- evidence: https://api.filedone.ai/.well-known/oauth-authorization-server
  flows:
    authorizationCode:
      authorization_url: https://api.filedone.ai/oauth/authorize
      client_id_metadata_document: true
      code_challenge_methods:
      - S256
      dynamic_client_registration: true
      grant_types:
      - authorization_code
      - refresh_token
      pkce: required
      registration_url: https://api.filedone.ai/oauth/register
      response_types:
      - code
      revocation_url: https://api.filedone.ai/oauth/revoke
      scopes:
      - tools:run
      - offline_access
      token_endpoint_auth_methods:
      - none
      token_url: https://api.filedone.ai/oauth/token
  name: oauth2
  type: oauth2
- bearer_format: fdk_<opaque>
  description: 'API key issued on the user''s filedone account page under "API keys". Sent as "Authorization: Bearer fdk_your_key". Keys are shown once; an account may hold up to five at a time and can revoke a key from the account page.'
  evidence: https://filedone.ai/developers
  name: bearer_api_key
  scheme: bearer
  type: http
slug: filedone-ai-authentication
source_filename: filedone-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://filedone.ai/developers
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filedone.ai/developers\nsources:\n- https://filedone.ai/developers\n- https://api.filedone.ai/.well-known/oauth-protected-resource\n- https://api.filedone.ai/.well-known/oauth-authorization-server\n- https://api.filedone.ai/mcp/server-card\ndocs: https://filedone.ai/developers\nname: filedone authentication\nsummary: >-\n  filedone's remote MCP server at https://api.filedone.ai/mcp accepts one of\n  two credentials. The standard flow is OAuth 2.1 with PKCE: the server\n  advertises OAuth 2.0 Protected Resource Metadata (RFC 9728) at\n  /.well-known/oauth-protected-resource and an authorization server at\n  https://api.filedone.ai, which supports Dynamic Client Registration\n  (RFC 7591), Client ID Metadata Documents, and PKCE with S256. Alternatively\n  a request may carry \"Authorization: Bearer fdk_<key>\" with an API key\n  minted from the signed-in user's account page. An account can hold up to\n  five keys and\
  \ a key is shown exactly once.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorization_url: https://api.filedone.ai/oauth/authorize\n      token_url: https://api.filedone.ai/oauth/token\n      registration_url: https://api.filedone.ai/oauth/register\n      revocation_url: https://api.filedone.ai/oauth/revoke\n      grant_types:\n      - authorization_code\n      - refresh_token\n      response_types:\n      - code\n      code_challenge_methods:\n      - S256\n      token_endpoint_auth_methods:\n      - none\n      scopes:\n      - tools:run\n      - offline_access\n      pkce: required\n      dynamic_client_registration: true\n      client_id_metadata_document: true\n  evidence: https://api.filedone.ai/.well-known/oauth-authorization-server\n- name: bearer_api_key\n  type: http\n  scheme: bearer\n  bearer_format: fdk_<opaque>\n  description: >-\n    API key issued on the user's filedone account page under \"API keys\".\n    Sent as \"Authorization:\
  \ Bearer fdk_your_key\". Keys are shown once; an\n    account may hold up to five at a time and can revoke a key from the\n    account page.\n  evidence: https://filedone.ai/developers\nprotected_resource_metadata: https://api.filedone.ai/.well-known/oauth-protected-resource\nmcp_endpoint: https://api.filedone.ai/mcp\nnotes:\n- The protected-resource metadata lists bearer_methods_supported = [\"header\"]\n  only; credentials are never accepted on the query string.\n- The authorization server's token endpoint uses token_endpoint_auth_method\n  \"none\" (a public client with PKCE).\n"
source_yaml_url: https://artifacts.apis.io/filedone-ai/authentication/filedone-ai-authentication.yml
summary_line: 2 schemes
tags:
- PDF
- Image Processing
- Document Conversion
- OCR
- AI Tools
- File Compression
- MCP
- Productivity
---
