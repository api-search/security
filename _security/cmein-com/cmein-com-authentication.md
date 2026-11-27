---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: CMeIn Authentication
name_suffix: Authentication
oauth_flows: []
overview: CMeIn declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CMeIn
provider_slug: cmein-com
scheme_count: 2
schemes:
- applies_to:
  - photo_advice
  - cmein_pricing
  - see_examples
  - find_video
  - cmein_info
  - contact_us
  evidence: '"Paste the address above and six tools work straight away, with nothing to sign in to." (https://cmein.com/mcp)'
  name: anonymous
  type: none
- applies_to:
  - my_credits
  - my_generations
  - find_scene
  - request_credits_back
  authorization_endpoint: https://cmein.com/oauth/authorize
  authorization_server_metadata: https://cmein.com/.well-known/oauth-authorization-server
  bearer_methods:
  - header
  dynamic_client_registration: true
  flows:
  - authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://cmein.com
  jwks_uri: https://cmein.com/.well-known/jwks.json
  name: cmein-oauth
  pkce: S256
  protected_resource_metadata: https://mcp.cmein.com/.well-known/oauth-protected-resource
  registration_endpoint: https://cmein.com/oauth/register
  resource_indicators_supported: true
  revocation_endpoint: https://cmein.com/oauth/revoke
  revocation_note: '"you can disconnect any assistant from your account settings, which takes full effect within fifteen minutes." (https://cmein.com/mcp)'
  token_endpoint: https://cmein.com/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: cmein-com-authentication
source_filename: cmein-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CMeIn authentication\ngenerated: '2026-11-04'\nmethod: probed\nsource:\n- https://mcp.cmein.com/.well-known/oauth-protected-resource\n- https://cmein.com/.well-known/oauth-authorization-server\n- https://cmein.com/mcp\ndocs: https://cmein.com/mcp\nnote: CMeIn publishes no REST API. The only programmable surface is the remote MCP server at https://mcp.cmein.com/mcp. Six tools answer anonymously; four (my_credits, my_generations, find_scene, request_credits_back) need an OAuth 2.0 bearer token for a connected CMeIn account. Discovery documents read with GET on 2026-11-04 (both HTTP 200). No auth, token or registration endpoint was called.\nschemes:\n- name: anonymous\n  type: none\n  applies_to: [photo_advice, cmein_pricing, see_examples, find_video, cmein_info, contact_us]\n  evidence: '\"Paste the address above and six tools work straight away, with nothing to sign in to.\" (https://cmein.com/mcp)'\n- name: cmein-oauth\n  type: oauth2\n  flows: [authorization_code]\n\
  \  pkce: S256\n  token_endpoint_auth_methods: [none]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  issuer: https://cmein.com\n  authorization_endpoint: https://cmein.com/oauth/authorize\n  token_endpoint: https://cmein.com/oauth/token\n  registration_endpoint: https://cmein.com/oauth/register\n  revocation_endpoint: https://cmein.com/oauth/revoke\n  jwks_uri: https://cmein.com/.well-known/jwks.json\n  dynamic_client_registration: true\n  resource_indicators_supported: true\n  bearer_methods: [header]\n  protected_resource_metadata: https://mcp.cmein.com/.well-known/oauth-protected-resource\n  authorization_server_metadata: https://cmein.com/.well-known/oauth-authorization-server\n  applies_to: [my_credits, my_generations, find_scene, request_credits_back]\n  revocation_note: '\"you can disconnect any assistant from your account settings, which takes full effect within fifteen minutes.\" (https://cmein.com/mcp)'\n"
source_yaml_url: https://artifacts.apis.io/cmein-com/authentication/cmein-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Image Generation
- Photos
- Dating
- Headshots
- Consumer App
- MCP
---
