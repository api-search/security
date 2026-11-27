---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cluvi AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cluvi AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cluvi AI
provider_slug: cluvi-ai
scheme_count: 1
schemes:
- applies_to: https://cluvi.ai/mcp
  authorization_url: https://cluvi.ai/oauth/authorize
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  code_challenge_methods:
  - S256
  evidence:
  - quote: 'Sign-in: OAuth 2.1 against Cluvi AI (discovery from the 401, client ID metadata documents or dynamic registration, PKCE). There is no API key'
    url: https://cluvi.ai/mcp.md
  - http_status: 200
    url: https://cluvi.ai/.well-known/oauth-authorization-server
  - http_status: 200
    url: https://cluvi.ai/.well-known/oauth-protected-resource/mcp
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://cluvi.ai
  name: cluviOAuth
  pkce: required
  registration_url: https://cluvi.ai/oauth/register
  revocation_url: https://cluvi.ai/oauth/revoke
  scopes:
  - mcp:read
  - mcp:write
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  token_url: https://cluvi.ai/oauth/token
  type: oauth2
slug: cluvi-ai-authentication
source_filename: cluvi-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cluvi.ai/mcp.md\ndocs: https://cluvi.ai/mcp.md\nsummary: The only programmatic surface is the remote MCP server at https://cluvi.ai/mcp. It uses OAuth 2.1 authorization code with PKCE (S256) against cluvi.ai. Clients identify themselves with client ID metadata documents or dynamic client registration. The docs say \"There is no API key\". An unauthenticated call returns 401, and the discovery metadata is reached from that 401.\nschemes:\n- name: cluviOAuth\n  type: oauth2\n  flow: authorizationCode\n  pkce: required\n  code_challenge_methods: [S256]\n  issuer: https://cluvi.ai\n  authorization_url: https://cluvi.ai/oauth/authorize\n  token_url: https://cluvi.ai/oauth/token\n  registration_url: https://cluvi.ai/oauth/register\n  revocation_url: https://cluvi.ai/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n  client_id_metadata_document_supported:\
  \ true\n  bearer_methods: [header]\n  scopes: [mcp:read, mcp:write]\n  applies_to: https://cluvi.ai/mcp\n  evidence:\n  - url: https://cluvi.ai/mcp.md\n    quote: 'Sign-in: OAuth 2.1 against Cluvi AI (discovery from the 401, client ID metadata documents or dynamic registration, PKCE). There is no API key'\n  - url: https://cluvi.ai/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://cluvi.ai/.well-known/oauth-protected-resource/mcp\n    http_status: 200\nnote: The endpoint URLs come from the published RFC 8414 / RFC 9728 metadata, which was read with a GET. None of the OAuth endpoints were called.\n"
source_yaml_url: https://artifacts.apis.io/cluvi-ai/authentication/cluvi-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Restaurant
- Hospitality
- Reservations
- WhatsApp
- Messaging
- AI Receptionist
- MCP
---
