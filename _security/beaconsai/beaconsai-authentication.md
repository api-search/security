---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Beaconsai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beacons.ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Beacons.ai
provider_slug: beaconsai
scheme_count: 1
schemes:
- applies_to:
  - https://beacons.ai/api/v001/creator/mcp
  authorization_url: https://beacons.ai/api/v001/oauth/authorize
  bearer_methods:
  - header
  dynamic_client_registration: true
  flow: authorizationCode
  grant_types:
  - authorization_code
  id: beacons_oauth
  issuer: https://beacons.ai
  note: '"none" in token_endpoint_auth_methods is the public-client case that pairs with PKCE — it is the expected shape for an MCP client, not a missing credential check. No refresh_token grant is advertised, so a token is not documented as renewable without re-consent.'
  pkce: required
  pkce_methods:
  - S256
  registration_url: https://beacons.ai/api/v001/oauth/register
  response_types:
  - code
  scopes:
  - description: The only scope the authorization server advertises. Read access to the creator MCP resource. Beacons publishes no scope reference page, so no further description is available and none has been invented.
    name: mcp:read
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  token_url: https://beacons.ai/api/v001/oauth/token
  type: oauth2
slug: beaconsai-authentication
source_filename: beaconsai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://beacons.ai/.well-known/oauth-authorization-server (RFC 8414, 200),\n  https://beacons.ai/.well-known/oauth-protected-resource (RFC 9728, 200), and the\n  WWW-Authenticate challenge returned by\n  https://beacons.ai/api/v001/creator/mcp\nsummary: >-\n  Beacons.ai has no documented API authentication page. Everything below is read\n  from the two machine-readable OAuth discovery documents the platform actually\n  serves. They describe a single OAuth 2.1 authorization server at\n  https://beacons.ai protecting one resource — the Creator MCP endpoint.\nschemes:\n- id: beacons_oauth\n  type: oauth2\n  flow: authorizationCode\n  pkce: required\n  pkce_methods: [S256]\n  issuer: https://beacons.ai\n  authorization_url: https://beacons.ai/api/v001/oauth/authorize\n  token_url: https://beacons.ai/api/v001/oauth/token\n  registration_url: https://beacons.ai/api/v001/oauth/register\n  dynamic_client_registration: true\n  response_types:\
  \ [code]\n  grant_types: [authorization_code]\n  token_endpoint_auth_methods: [none, client_secret_post]\n  scopes:\n  - name: mcp:read\n    description: >-\n      The only scope the authorization server advertises. Read access to the\n      creator MCP resource. Beacons publishes no scope reference page, so no\n      further description is available and none has been invented.\n  applies_to:\n  - https://beacons.ai/api/v001/creator/mcp\n  bearer_methods: [header]\n  note: >-\n    \"none\" in token_endpoint_auth_methods is the public-client case that pairs with\n    PKCE — it is the expected shape for an MCP client, not a missing credential\n    check. No refresh_token grant is advertised, so a token is not documented as\n    renewable without re-consent.\nnot_found:\n- api-key issuance page\n- personal access tokens\n- OpenID Connect discovery (/.well-known/openid-configuration returns 404)\n- mutual TLS\n- any human-readable authentication documentation on beacons.ai or\n  help.beacons.ai\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconsai/refs/heads/main/authentication/beaconsai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Creator Economy
- Link in Bio
- Creator Website Builder
- Creator Storefront
- Media Kit
- Email Marketing
- Affiliate Marketing
- Creator Monetization
- Influencer Software
- MCP
- agent-native
---
