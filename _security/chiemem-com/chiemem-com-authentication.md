---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chiemem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chiemem declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Chiemem
provider_slug: chiemem-com
scheme_count: 1
schemes:
- applies_to: https://chiemem.com/mcp
  authorization_endpoint: https://chiemem.com/authorize
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  documented_behaviour:
  - The seller logs in to Chiemem and approves the connection on Chiemem's consent screen; the AI app never receives the Chiemem password or Google account details, only a key usable for this connection.
  - Connections can be revoked from My Page (AI アプリとの連携); a connection unused for 90 days is disconnected automatically.
  - Connections made before 2026-10-10 lack the publishing consent and must be removed and reconnected to publish.
  dynamic_client_registration: true
  evidence:
  - http_status: 200
    url: https://chiemem.com/.well-known/oauth-authorization-server
  - http_status: 200
    url: https://chiemem.com/.well-known/oauth-protected-resource/mcp
  flows:
  - authorization_code
  - refresh_token
  name: chiemem-oauth
  pkce: S256
  registration_endpoint: https://chiemem.com/oauth/register
  revocation_endpoint: https://chiemem.com/oauth/token
  scopes:
  - chiemem:publish
  token_endpoint: https://chiemem.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: chiemem-com-authentication
source_filename: chiemem-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Chiemem authentication\ngenerated: '2026-11-03'\nmethod: searched\nsource: https://chiemem.com/guide/ai/\ndocs: https://chiemem.com/guide/ai/\nnote: No OpenAPI is published; the profile is read from the guide page and from the OAuth metadata documents the provider publishes (RFC 8414 / RFC 9728). Only the MCP server at https://chiemem.com/mcp is protected this way; it answers 401 without a bearer token.\nschemes:\n- name: chiemem-oauth\n  type: oauth2\n  flows:\n  - authorization_code\n  - refresh_token\n  pkce: S256\n  authorization_endpoint: https://chiemem.com/authorize\n  token_endpoint: https://chiemem.com/oauth/token\n  revocation_endpoint: https://chiemem.com/oauth/token\n  registration_endpoint: https://chiemem.com/oauth/register\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  scopes: [chiemem:publish]\n  bearer_methods: [header]\n  applies_to:\
  \ https://chiemem.com/mcp\n  evidence:\n  - url: https://chiemem.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://chiemem.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n  documented_behaviour:\n  - The seller logs in to Chiemem and approves the connection on Chiemem's consent screen; the AI app never receives the Chiemem password or Google account details, only a key usable for this connection.\n  - Connections can be revoked from My Page (AI アプリとの連携); a connection unused for 90 days is disconnected automatically.\n  - Connections made before 2026-10-10 lack the publishing consent and must be removed and reconnected to publish.\n"
source_yaml_url: https://artifacts.apis.io/chiemem-com/authentication/chiemem-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Marketplace
- Prompts
- Artificial Intelligence
- Generative AI
- Digital Content
- Japan
- MCP
---
