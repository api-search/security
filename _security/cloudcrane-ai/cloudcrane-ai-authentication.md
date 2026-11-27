---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: CloudCrane Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudCrane declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CloudCrane
provider_slug: cloudcrane-ai
scheme_count: 1
schemes:
- bearer_methods:
  - header
  description: MCP clients connect over OAuth with PKCE and dynamic client registration ("there's no key to paste and nothing to add to its headers"). The user signs in with Google or a code sent by email, picks a workspace they own, and approves the assistant. Only a workspace owner can connect an assistant; owners can sign an assistant out at any time and "its access ends at once". Keys are kept only as hashes.
  dynamic_client_registration: true
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://cloudcrane.ai
  name: oauth2
  pkce: S256
  resource: https://cloudcrane.ai/api/apps/mcp
  scopes:
  - apps:read
  - apps:write
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: cloudcrane-ai-authentication
source_filename: cloudcrane-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource:\n- https://cloudcrane.ai/.well-known/oauth-protected-resource\n- https://cloudcrane.ai/.well-known/oauth-authorization-server\n- https://cloudcrane.ai/docs/connect\n- https://cloudcrane.ai/security\n- https://github.com/cloudcrane-dev/cloudcrane-mcp\ndocs: https://cloudcrane.ai/docs/connect\nnote: No OpenAPI is published; the profile comes from the provider's OAuth discovery documents (both HTTP 200 on GET, 2026-11-04) and its docs. Token, registration and authorize endpoints were not called.\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none]\n  dynamic_client_registration: true\n  issuer: https://cloudcrane.ai\n  bearer_methods: [header]\n  resource: https://cloudcrane.ai/api/apps/mcp\n  scopes: [apps:read, apps:write]\n  description: 'MCP clients connect over OAuth with PKCE and dynamic client registration\
  \ (\"there''s no key to paste and nothing to add to its headers\"). The user signs in with Google or a code sent by email, picks a workspace they own, and approves the assistant. Only a workspace owner can connect an assistant; owners can sign an assistant out at any time and \"its access ends at once\". Keys are kept only as hashes.'\nuser_sign_in: [Google, email one-time code]\n"
source_yaml_url: https://artifacts.apis.io/cloudcrane-ai/authentication/cloudcrane-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Assistant
- MCP
- Mobile App
- No-Code
- App Builder
- Progressive Web Apps
---
