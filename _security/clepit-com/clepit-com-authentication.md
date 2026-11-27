---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Clepit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clepit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clepit
provider_slug: clepit-com
scheme_count: 1
schemes:
- applies_to: https://api.clepit.com/mcp (remote streamable-HTTP MCP server com.clepit/mcp); the documented-by-preflight GraphQL endpoint https://api.clepit.com/graphql also answers 401 anonymously
  authorization_endpoint: https://auth.bomdisoft.com/oauth/v2/authorize
  authorization_server: https://auth.bomdisoft.com
  bearer: true
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:device_code
  name: oauth2-mcp
  openid_configuration: https://auth.bomdisoft.com/.well-known/openid-configuration
  pkce: S256
  protected_resource_metadata: https://api.clepit.com/.well-known/oauth-protected-resource
  registration_endpoint: https://auth.bomdisoft.com/oauth/v2/register
  scopes_supported:
  - openid
  - email
  - urn:zitadel:iam:org:project:id:377023715914839692:aud
  token_endpoint: https://auth.bomdisoft.com/oauth/v2/token
  type: oauth2
slug: clepit-com-authentication
source_filename: clepit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource:\n- https://api.clepit.com/.well-known/oauth-protected-resource\n- https://auth.bomdisoft.com/.well-known/openid-configuration\n- https://registry.modelcontextprotocol.io/v0/servers?search=clepit\nschemes:\n- name: oauth2-mcp\n  type: oauth2\n  applies_to: https://api.clepit.com/mcp (remote streamable-HTTP MCP server com.clepit/mcp); the documented-by-preflight GraphQL endpoint https://api.clepit.com/graphql also answers 401 anonymously\n  bearer: true\n  protected_resource_metadata: https://api.clepit.com/.well-known/oauth-protected-resource\n  authorization_server: https://auth.bomdisoft.com\n  openid_configuration: https://auth.bomdisoft.com/.well-known/openid-configuration\n  authorization_endpoint: https://auth.bomdisoft.com/oauth/v2/authorize\n  token_endpoint: https://auth.bomdisoft.com/oauth/v2/token\n  registration_endpoint: https://auth.bomdisoft.com/oauth/v2/register\n  grant_types_supported: [authorization_code, implicit,\
  \ refresh_token, client_credentials, 'urn:ietf:params:oauth:grant-type:jwt-bearer', 'urn:ietf:params:oauth:grant-type:device_code']\n  pkce: S256\n  scopes_supported: [openid, email, 'urn:zitadel:iam:org:project:id:377023715914839692:aud']\nnote: Read from unauthenticated GETs of the published discovery documents only; no token, login or registration endpoint was called. The clepit.com docs cover only the in-process @clepit/core library and publish no authentication page for the cloud API. The pricing page lists \"API, GraphQL, MCP and agents\" under Platform.\n"
source_yaml_url: https://artifacts.apis.io/clepit-com/authentication/clepit-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Block Editor
- Rich Text Editor
- Knowledge Base
- Open Source
- TypeScript
- JSON
- Collaboration
- Wiki
---
