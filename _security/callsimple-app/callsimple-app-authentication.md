---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: CallSimple Authentication
name_suffix: Authentication
oauth_flows: []
overview: CallSimple declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CallSimple
provider_slug: callsimple-app
scheme_count: 1
schemes:
- applies_to: https://callsimple.app/mcp
  authorization_endpoint: https://callsimple.app/oauth/authorize
  bearer_methods:
  - header
  evidence:
  - http_status: 200
    url: https://callsimple.app/.well-known/oauth-protected-resource
  - http_status: 200
    url: https://callsimple.app/.well-known/oauth-authorization-server
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://callsimple.app
  name: oauth2
  pkce: S256
  registration_endpoint: https://callsimple.app/oauth/register
  scopes:
  - calls
  - offline_access
  token_endpoint: https://callsimple.app/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: callsimple-app-authentication
source_filename: callsimple-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: https://callsimple.app/.well-known/oauth-authorization-server\ndocs: https://callsimple.app/claude\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  issuer: https://callsimple.app\n  authorization_endpoint: https://callsimple.app/oauth/authorize\n  token_endpoint: https://callsimple.app/oauth/token\n  registration_endpoint: https://callsimple.app/oauth/register\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none]\n  bearer_methods: [header]\n  scopes: [calls, offline_access]\n  applies_to: https://callsimple.app/mcp\n  evidence:\n  - url: https://callsimple.app/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://callsimple.app/.well-known/oauth-authorization-server\n    http_status: 200\nnote: Read from the published RFC 9728 protected-resource and RFC 8414 authorization-server metadata (GET only; the OAuth endpoints themselves\
  \ were not called). The connector guides describe the end-user flow as signing in with a phone number verified by a call-back code, then pressing Allow on a CallSimple consent page; ChatGPT's custom MCP app \"Authentication already says OAuth\". The MCP endpoint answers 401 without a token.\n"
source_yaml_url: https://artifacts.apis.io/callsimple-app/authentication/callsimple-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Voice Agents
- Phone Calls
- MCP
- ChatGPT Apps
- Claude Connectors
- Voice
- India
---
