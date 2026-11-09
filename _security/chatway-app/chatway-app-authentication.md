---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chatway-app-openapi-generated.yml
  format: yaml
  label: Chatway API
  slug: chatway-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatway-app/openapi/_ae-authored/chatway-app-openapi-generated.yml
auth_types: []
description: Authentication methods for Chatway API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chatway App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chatway declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chatway
provider_slug: chatway-app
scheme_count: 2
schemes:
- evidence: 'Include your API key in the X-API-KEY header with every request:'
  header: X-API-KEY
  how_to_obtain: Generate an API key in the Chatway dashboard under Settings → Developer Tools → API Keys.
  location: header
  name: API Key
  type: apiKey
- authorize_url: https://mcp.chatway.app/oauth/authorize
  evidence: OAuth discovery metadata tells an MCP client where to begin sign-in and which authorization features the server supports.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Use the protected‑resource metadata at https://mcp.chatway.app/.well-known/oauth-protected-resource/mcp and follow its authorization‑server link to obtain tokens.
  name: OAuth
  scopes:
  - mcp:use
  type: oauth2
slug: chatway-app-authentication
source_filename: chatway-app-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.chatway.app/operations/apiDocs.apiDocsAuthMd
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.chatway.app/operations/apiDocs.apiDocsAuthMd\nsources:\n- https://developers.chatway.app/operations/apiDocs.apiDocsAuthMd\n- https://developers.chatway.app/operations/apiDocs.apiDocsOAuthMetadata\n- https://developers.chatway.app/operations/guides.quickstart\ndescription: Authentication methods for Chatway API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Include your API key in the X-API-KEY header with every request:'\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Generate an API key in the Chatway dashboard under Settings → Developer Tools → API Keys.\n- type: oauth2\n  name: OAuth\n  evidence: OAuth discovery metadata tells an MCP client where to begin sign-in and which authorization features the server supports.\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://mcp.chatway.app/oauth/authorize\n  scopes:\n\
  \  - mcp:use\n  how_to_obtain: Use the protected‑resource metadata at https://mcp.chatway.app/.well-known/oauth-protected-resource/mcp and follow its authorization‑server\n    link to obtain tokens.\ndocs: https://developers.chatway.app/operations/apiDocs.apiDocsAuthMd\n"
source_yaml_url: https://artifacts.apis.io/chatway-app/authentication/chatway-app-authentication.yml
summary_line: 2 schemes
tags:
- Live Chat
- Artificial Intelligence
- Customer Service
- MCP
- Chatbots
- Company
---
