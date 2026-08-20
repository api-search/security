---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: View Com Au Authentication
name_suffix: Authentication
oauth_flows: []
overview: View.com.au secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: View.com.au
provider_slug: view-com-au
scheme_count: 1
schemes:
- applies_to: view-com-au-property-mcp-server
  description: The MCP server accepts anonymous JSON-RPC with no Authorization header, no API key, no session, no account and no agreement. initialize, tools/list and tools/call all succeed for any caller. Verified 2026-07-26.
  evidence:
  - probe: POST https://mcp.view.com.au/mcp tools/list
    status: 200
  - probe: POST https://mcp.view.com.au/mcp tools/call propertySearch
    status: 200
  name: none
  surface: https://mcp.view.com.au/mcp
  type: none
slug: view-com-au-authentication
source_filename: view-com-au-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live probes of mcp.view.com.au, api.view.com.au, sandbox.api.view.com.au and view.com.au\nnotes: >-\n  There is no OpenAPI to derive security schemes from, and no published\n  authentication documentation of any kind. This profile is assembled from live\n  anonymous probes on 2026-07-26. The result is a split posture: the reachable\n  agent surface has no authentication at all, while every other API host\n  rejects unauthenticated callers with no published way to obtain credentials.\n\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  public_surface: unauthenticated\n  gated_surfaces: 2\n  scopes_artifact: null    # no OAuth, so scopes/ is intentionally absent\n\nschemes:\n- name: none\n  type: none\n  surface: https://mcp.view.com.au/mcp\n  applies_to: view-com-au-property-mcp-server\n  description: >-\n    The MCP server accepts anonymous JSON-RPC with no Authorization header, no\n    API key, no session, no\
  \ account and no agreement. initialize, tools/list\n    and tools/call all succeed for any caller. Verified 2026-07-26.\n  evidence:\n  - {probe: 'POST https://mcp.view.com.au/mcp tools/list', status: 200}\n  - {probe: 'POST https://mcp.view.com.au/mcp tools/call propertySearch', status: 200}\n\ngated_surfaces:\n- host: https://api.view.com.au\n  mechanism: AWS API Gateway native authorization (IAM / custom authorizer / usage-plan key — indeterminate from outside)\n  challenge: 'HTTP 403 with x-amzn-errortype: MissingAuthenticationTokenException'\n  documented: false\n  onboarding_path: none published\n  evidence:\n  - {probe: 'https://api.view.com.au/v1', status: 403}\n  - {probe: 'https://api.view.com.au/openapi.json', status: 403}\n- host: https://sandbox.api.view.com.au\n  mechanism: same AWS API Gateway posture as production\n  challenge: HTTP 403 application/json\n  documented: false\n  onboarding_path: none published\n  evidence:\n  - {probe: 'https://sandbox.api.view.com.au/openapi.json',\
  \ status: 403}\n\ndiscovery_probes:\n- {url: 'https://mcp.view.com.au/.well-known/oauth-authorization-server', status: 404}\n- {url: 'https://mcp.view.com.au/.well-known/oauth-protected-resource', status: 404}\n- {url: 'https://mcp.view.com.au/.well-known/openid-configuration', status: 404}\n- {url: 'https://view.com.au/.well-known/openid-configuration', status: 403, note: DataDome challenge, not an OIDC document}\n- {url: 'https://api.view.com.au/.well-known/openid-configuration', status: 403}\n\nend_user_auth:\n  note: >-\n    The consumer website offers account sign-up via Google, Apple or one-time\n    password, and agencies sign up through the agency hub. Neither is an API\n    credential — no developer can convert either into machine access.\n  sign_up: https://view.com.au/agency-hub/signup/\n\nagent_guidance: >-\n  Send no credentials. Adding an Authorization header is unnecessary and there\n  is no credential to add. The absence of authentication also means the absence\n  of identity:\
  \ an agent cannot be attributed, cannot request a quota increase,\n  and cannot appeal a block. Budget against the 100-request / 300-second\n  anonymous rate limit in rate-limits/view-com-au-rate-limits.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/view-com-au/refs/heads/main/authentication/view-com-au-authentication.yml
summary_line: none · 1 scheme
tags:
- Real-Estate
- Australia
- Property Listings
- Property Portal
- PropTech
- Rentals
- Off-Market Property Data
- MCP
- agent-native
---
