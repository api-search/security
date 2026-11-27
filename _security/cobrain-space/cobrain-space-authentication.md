---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cobrain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cobrain declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cobrain
provider_slug: cobrain-space
scheme_count: 1
schemes:
- applies_to: https://cobrain.space/mcp
  authorization_server_metadata: https://cobrain.space/.well-known/oauth-authorization-server
  dynamic_client_registration: https://cobrain.space/oauth/register
  flows:
  - authorization_code
  - refresh_token
  issuer: https://cobrain.space
  name: oauth2
  pkce: S256
  protected_resource: https://cobrain.space/mcp
  protected_resource_metadata: https://cobrain.space/.well-known/oauth-protected-resource
  scopes:
  - openid
  - profile
  - email
  - offline_access
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: cobrain-space-authentication
source_filename: cobrain-space-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cobrain.space/guides/tools\ndocs: https://cobrain.space/guides/tools\nsummary: 'The only programmatic surface is the remote MCP server https://cobrain.space/mcp (Streamable HTTP). \"A standard remote MCP server, with OAuth 2.1 ... The program registers itself, the user authorises on a Cobrain page that states what the program will be able to do, and it receives a grant that expires and renews. No API key.\" Every tool runs with the identity of the authorising user; revoking from the Connections page refuses every later call. Discovery documents were read with GET (2026-11-04): /.well-known/oauth-protected-resource (200) and /.well-known/oauth-authorization-server (200); /.well-known/openid-configuration 404. The anonymous MCP endpoint answers 401 (pre-flight dossier).'\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - authorization_code\n  - refresh_token\n  pkce: S256\n  dynamic_client_registration: https://cobrain.space/oauth/register\n\
  \  issuer: https://cobrain.space\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  scopes: [openid, profile, email, offline_access]\n  protected_resource: https://cobrain.space/mcp\n  protected_resource_metadata: https://cobrain.space/.well-known/oauth-protected-resource\n  authorization_server_metadata: https://cobrain.space/.well-known/oauth-authorization-server\n  applies_to: https://cobrain.space/mcp\napi_keys: none\napi_keys_evidence: '\"If it asks for an API key, there is none: ask it for a remote MCP server over HTTP with OAuth.\"'\n"
source_yaml_url: https://artifacts.apis.io/cobrain-space/authentication/cobrain-space-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Memory
- MCP
- MCP Server
- Knowledge Management
- Markdown
- Note Taking
- Collaboration
- Artificial Intelligence
---
