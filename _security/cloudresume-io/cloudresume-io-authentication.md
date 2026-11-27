---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: cloudresume.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: cloudresume.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: cloudresume.io
provider_slug: cloudresume-io
scheme_count: 1
schemes:
- applies_to: https://cloudresume.io/api/mcp
  authorization_server_metadata: https://cloudresume.io/.well-known/oauth-authorization-server
  bearer_format: access token (urn:ietf:params:oauth:token-type:access_token)
  description: The MCP server "authenticates against your existing login"; the first call prompts the user to authorize the agent against their account. Anonymous calls receive 401 with a Bearer resource_metadata challenge.
  dynamic_client_registration: true
  flows:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  identity_provider: Clerk (clerk.cloudresume.io)
  issuer: https://cloudresume.io
  jwks_uri: https://clerk.cloudresume.io/.well-known/jwks.json
  name: oauth2
  pkce: S256
  token_endpoint_auth_methods:
  - client_secret_basic
  - none
  - client_secret_post
  type: oauth2
slug: cloudresume-io-authentication
source_filename: cloudresume-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://cloudresume.io/.well-known/oauth-protected-resource\ndocs: https://cloudresume.io/blog/how-to-use-your-ai-agent-to-manage-your-resumes\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://cloudresume.io/api/mcp\n  description: The MCP server \"authenticates against your existing login\"; the first call prompts the user to authorize the\n    agent against their account. Anonymous calls receive 401 with a Bearer resource_metadata challenge.\n  bearer_format: access token (urn:ietf:params:oauth:token-type:access_token)\n  identity_provider: Clerk (clerk.cloudresume.io)\n  authorization_server_metadata: https://cloudresume.io/.well-known/oauth-authorization-server\n  issuer: https://cloudresume.io\n  flows:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  pkce: S256\n  dynamic_client_registration: true\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  -\
  \ none\n  - client_secret_post\n  jwks_uri: https://clerk.cloudresume.io/.well-known/jwks.json\napi_keys: none documented\n"
source_yaml_url: https://artifacts.apis.io/cloudresume-io/authentication/cloudresume-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Resume
- Resume Builder
- Careers
- Artificial Intelligence
- Cover Letters
- JSON Resume
- MCP
---
