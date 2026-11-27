---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: CoverTheGaps Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoverTheGaps declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CoverTheGaps
provider_slug: coverthegaps-com
scheme_count: 1
schemes:
- applies_to: https://coverthegaps.com/mcp
  authorizationUrl: https://coverthegaps.com/o/authorize/
  authorization_server: https://coverthegaps.com
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  flows:
  - authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  introspectionUrl: https://coverthegaps.com/o/introspect/
  name: CoverTheGaps MCP OAuth
  pkce:
  - S256
  protected_resource: https://coverthegaps.com/.well-known/oauth-protected-resource
  registrationUrl: https://coverthegaps.com/o/register/
  revocationUrl: https://coverthegaps.com/o/revoke_token/
  scopes:
  - mcp:read
  - mcp:write
  - offline_access
  tokenUrl: https://coverthegaps.com/o/token/
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: coverthegaps-com-authentication
source_filename: coverthegaps-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://coverthegaps.com/.well-known/oauth-authorization-server\ndocs: https://coverthegaps.com/agents/\nsummary: >-\n  The CoverTheGaps MCP server (https://coverthegaps.com/mcp) is an OAuth 2.0 protected resource. Its RFC 9728\n  protected-resource metadata (HTTP 200) names https://coverthegaps.com as the authorization server and\n  accepts bearer tokens in the header only. The RFC 8414 authorization-server metadata (HTTP 200) advertises the\n  authorization_code and refresh_token grants with PKCE S256, dynamic client registration and client ID\n  metadata documents. Anonymous calls to /mcp return 401 (pre-flight). The docs describe the user flow as\n  \"One consent screen, on our site\" and say \"Reading and changing are asked for separately.\"\n  No token, registration or authorize endpoint was called.\nschemes:\n- name: CoverTheGaps MCP OAuth\n  type: oauth2\n  flows: [authorizationCode]\n  grant_types: [authorization_code,\
  \ refresh_token]\n  authorizationUrl: https://coverthegaps.com/o/authorize/\n  tokenUrl: https://coverthegaps.com/o/token/\n  revocationUrl: https://coverthegaps.com/o/revoke_token/\n  introspectionUrl: https://coverthegaps.com/o/introspect/\n  registrationUrl: https://coverthegaps.com/o/register/\n  pkce: [S256]\n  client_id_metadata_document_supported: true\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  bearer_methods: [header]\n  scopes: [mcp:read, mcp:write, offline_access]\n  protected_resource: https://coverthegaps.com/.well-known/oauth-protected-resource\n  authorization_server: https://coverthegaps.com\n  applies_to: https://coverthegaps.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/coverthegaps-com/authentication/coverthegaps-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Education
- Language Learning
- English Teaching
- Tutoring
- Homework
- MCP
- AI Assistant
---
