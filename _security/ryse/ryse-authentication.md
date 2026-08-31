---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Ryse Authentication
name_suffix: Authentication
oauth_flows: []
overview: RYSE declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: RYSE
provider_slug: ryse
scheme_count: 3
schemes:
- applies_to:
  - https://www.helloryse.com/api/ucp/mcp
  - https://www.helloryse.com/api/mcp
  description: tools/list, initialize, prompts/list and resources/list require no credential of any kind. Both endpoints returned HTTP 200 to an unauthenticated POST.
  evidence:
    date: '2026-08-26'
    http_status: 200
    probe: POST {"jsonrpc":"2.0","id":1,"method":"tools/list"}
  id: anonymous
  type: none
- applies_to:
  - https://www.helloryse.com/api/ucp/mcp
  description: 'Not authentication in the credential sense, but the UCP server''s admission control for tools/call: every request must carry meta["ucp-agent"].profile, a fetchable URI identifying the calling agent. The server dereferences it; a missing or unfetchable profile is rejected before the tool runs. This is the identity RYSE''s commerce surface actually checks.'
  evidence:
    body: '{"error":{"code":-32001,"message":"UCP discovery failed", "data":{"code":"invalid_profile_url","content":"Unable to fetch agent profile: Missing profile uri"}}}'
    date: '2026-08-26'
    http_status: 422
    probe: POST tools/call and prompts/list without meta["ucp-agent"].profile
  id: ucp-agent-profile
  parameter: meta.ucp-agent.profile
  parameter_format: uri
  required: true
  type: agent-identity
- applies_to:
  - https://account.helloryse.com/customer/api/mcp
  bearer_methods_supported:
  - header
  description: The customer-account MCP acts on a logged-in RYSE customer. tools/list is anonymous, but every tools/call requires a bearer access token issued by RYSE's customer authorization server.
  end_session_endpoint: https://account.helloryse.com/authentication/logout
  evidence:
    body: '{"errors":[{"message":"Unauthorized"}]}'
    date: '2026-08-26'
    http_status: 401
    probe: POST tools/call get_most_recent_order_status with no Authorization header
    www_authenticate: https://account.helloryse.com/authentication/.well-known/openid-configuration
  flows:
    authorization_code:
      authorization_url: https://account.helloryse.com/authentication/oauth/authorize
      code_challenge_methods_supported:
      - S256
      pkce: required
      token_url: https://account.helloryse.com/authentication/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: customer-oauth
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/51479806112
  jwks_uri: https://account.helloryse.com/authentication/.well-known/jwks.json
  response_types_supported:
  - code
  scopes_file: ../scopes/ryse-scopes.yml
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: ryse-authentication
source_filename: ryse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://account.helloryse.com/.well-known/oauth-authorization-server,\n  https://account.helloryse.com/.well-known/oauth-protected-resource,\n  https://www.helloryse.com/.well-known/openid-configuration, plus live anonymous and unauthenticated\n  JSON-RPC probes of all three RYSE MCP endpoints on 2026-08-26\nsummary: >-\n  RYSE publishes no API keys and no developer credentials. Its two commerce MCP surfaces on\n  www.helloryse.com are ANONYMOUS for discovery and for read/cart/checkout construction; the only\n  authenticated surface is the customer-account MCP on account.helloryse.com, which is protected by\n  RYSE's own OAuth 2.0 / OpenID Connect authorization server (Shopify-operated, merchant-scoped to\n  shop 51479806112) and advertises itself per RFC 9728.\nschemes:\n- id: anonymous\n  type: none\n  applies_to:\n  - https://www.helloryse.com/api/ucp/mcp\n  - https://www.helloryse.com/api/mcp\n  description: >-\n  \
  \  tools/list, initialize, prompts/list and resources/list require no credential of any kind. Both\n    endpoints returned HTTP 200 to an unauthenticated POST.\n  evidence:\n    probe: 'POST {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}'\n    http_status: 200\n    date: '2026-08-26'\n- id: ucp-agent-profile\n  type: agent-identity\n  applies_to:\n  - https://www.helloryse.com/api/ucp/mcp\n  description: >-\n    Not authentication in the credential sense, but the UCP server's admission control for\n    tools/call: every request must carry meta[\"ucp-agent\"].profile, a fetchable URI identifying the\n    calling agent. The server dereferences it; a missing or unfetchable profile is rejected before\n    the tool runs. This is the identity RYSE's commerce surface actually checks.\n  required: true\n  parameter: meta.ucp-agent.profile\n  parameter_format: uri\n  evidence:\n    probe: 'POST tools/call and prompts/list without meta[\"ucp-agent\"].profile'\n    http_status: 422\n  \
  \  body: >-\n      {\"error\":{\"code\":-32001,\"message\":\"UCP discovery failed\",\n      \"data\":{\"code\":\"invalid_profile_url\",\"content\":\"Unable to fetch agent profile: Missing profile uri\"}}}\n    date: '2026-08-26'\n- id: customer-oauth\n  type: oauth2\n  applies_to:\n  - https://account.helloryse.com/customer/api/mcp\n  description: >-\n    The customer-account MCP acts on a logged-in RYSE customer. tools/list is anonymous, but every\n    tools/call requires a bearer access token issued by RYSE's customer authorization server.\n  bearer_methods_supported:\n  - header\n  flows:\n    authorization_code:\n      authorization_url: https://account.helloryse.com/authentication/oauth/authorize\n      token_url: https://account.helloryse.com/authentication/oauth/token\n      pkce: required\n      code_challenge_methods_supported:\n      - S256\n  issuer: https://shopify.com/authentication/51479806112\n  jwks_uri: https://account.helloryse.com/authentication/.well-known/jwks.json\n\
  \  end_session_endpoint: https://account.helloryse.com/authentication/logout\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  response_types_supported:\n  - code\n  id_token_signing_alg_values_supported:\n  - RS256\n  scopes_file: ../scopes/ryse-scopes.yml\n  evidence:\n    probe: 'POST tools/call get_most_recent_order_status with no Authorization header'\n    http_status: 401\n    body: '{\"errors\":[{\"message\":\"Unauthorized\"}]}'\n    www_authenticate: https://account.helloryse.com/authentication/.well-known/openid-configuration\n    date: '2026-08-26'\nopenid_connect:\n  supported: true\n  discovery_document: https://account.helloryse.com/.well-known/openid-configuration\n  file: ../well-known/ryse-openid-configuration.json\n  subject_types_supported:\n  - public\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid,\
  \ email, email_verified]\nprotected_resource_metadata:\n  supported: true\n  standard: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  document: https://account.helloryse.com/.well-known/oauth-protected-resource\n  file: ../well-known/ryse-oauth-protected-resource.json\n  resource: https://account.helloryse.com\n  authorization_servers:\n  - https://account.helloryse.com\n  - https://shopify.com/authentication/51479806112\nnotes:\n- >-\n  No API key, no client credentials grant, and no machine-to-machine credential is published anywhere\n  on RYSE's own surface. An agent cannot obtain a RYSE-issued key.\n- >-\n  RYSE's robots.txt and agents.md impose an out-of-band authorization rule that no credential\n  satisfies: \"Checkouts are for humans. Do NOT complete checkout, payment, or order placement\n  automatically ... without an explicit, contemporaneous human approval step.\" Treat human approval\n  as a required authorization factor on complete_checkout.\n- >-\n  The device/hardware\
  \ side of RYSE (SmartShade, SmartCurtain, SmartBridge) has no published\n  authentication surface at all — there is no cloud or local device API documented for developers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ryse/refs/heads/main/authentication/ryse-authentication.yml
summary_line: 3 schemes
tags:
- Smart Home
- Internet of Things
- Consumer Electronics
- Home Automation
- Window Coverings
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- E-Commerce
- Shopify
---
