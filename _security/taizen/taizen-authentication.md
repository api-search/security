---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Taizen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taizen declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Taizen
provider_slug: taizen
scheme_count: 1
schemes:
- bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://eu.mcp.usetaizen.com/oauth/authorize
      scopes: {}
      tokenUrl: https://eu.mcp.usetaizen.com/oauth/token
  grant_types_supported:
  - authorization_code
  id: taizen-mcp-oauth2
  issuer: https://eu.mcp.usetaizen.com
  note: token_endpoint_auth_methods_supported is ["none"], i.e. public clients only — there is no confidential-client credential, and PKCE S256 is the sole proof of possession at the token endpoint. This is the expected shape for an MCP server talking to desktop/CLI agent clients.
  pkce_required: true
  public_client: true
  registration_endpoint: https://eu.mcp.usetaizen.com/oauth/register
  response_types_supported:
  - code
  scopes_supported: []
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: taizen-authentication
source_filename: taizen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://eu.mcp.usetaizen.com/.well-known/oauth-authorization-server and\n  https://eu.mcp.usetaizen.com/.well-known/oauth-protected-resource (both HTTP 200, probed\n  2026-08-14); 401 challenge headers on POST https://eu.mcp.usetaizen.com/mcp\nnote: >-\n  DERIVED FROM SERVED METADATA, NOT FROM AN OPENAPI. Taizen publishes no REST contract, so there are\n  no securitySchemes to read. Its only authenticated machine surface is the remote MCP server, which\n  implements the MCP OAuth profile properly: RFC 8414 authorization-server metadata, RFC 9728\n  protected-resource metadata, and an RFC 6750 WWW-Authenticate challenge that points a client at the\n  resource metadata document.\napplies_to:\n  api: Taizen MCP Server\n  resource: https://eu.mcp.usetaizen.com\nschemes:\n- id: taizen-mcp-oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://eu.mcp.usetaizen.com/oauth/authorize\n      tokenUrl:\
  \ https://eu.mcp.usetaizen.com/oauth/token\n      scopes: {}\n  issuer: https://eu.mcp.usetaizen.com\n  registration_endpoint: https://eu.mcp.usetaizen.com/oauth/register\n  dynamic_client_registration: true\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  bearer_methods_supported:\n  - header\n  scopes_supported: []\n  public_client: true\n  pkce_required: true\n  note: >-\n    token_endpoint_auth_methods_supported is [\"none\"], i.e. public clients only — there is no\n    confidential-client credential, and PKCE S256 is the sole proof of possession at the token\n    endpoint. This is the expected shape for an MCP server talking to desktop/CLI agent clients.\nchallenge:\n  status: 401\n  body: '{\"detail\":\"Missing or invalid Authorization header\"}'\n  www_authenticate: >-\n    Bearer resource_metadata=\"https://eu.mcp.usetaizen.com/.well-known/oauth-protected-resource\"\
  \n  cache_control: no-store\nscopes_published: false\nscopes_note: >-\n  scopes_supported is an empty array in BOTH metadata documents, so a client cannot request or reason\n  about least-privilege access — authorization is all-or-nothing against the connected Taizen\n  account. No scopes/ artifact is written for this repo because the provider publishes no scope\n  vocabulary of its own.\nconsumed_third_party_auth:\n  note: >-\n    Separately from the above, Taizen's docs describe the credentials Taizen ITSELF requests FROM the\n    customer's tools. These are inbound integration credentials, not scopes Taizen issues. Captured\n    in integrations/taizen-integrations.yml.\n  docs: https://docs.usetaizen.com/docs\nopenid_connect:\n  supported: false\n  evidence: >-\n    https://eu.mcp.usetaizen.com/.well-known/openid-configuration returns 404, as does the same path\n    on usetaizen.com, docs.usetaizen.com, api.usetaizen.com and us.mcp.usetaizen.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taizen/refs/heads/main/authentication/taizen-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Win-Loss Analysis
- Competitive Intelligence
- Sales Enablement
- Revenue Intelligence
- Go-To-Market
- AI Agents
- Battlecards
- Sales
- MCP
- Agent Skills
- Conversation Intelligence
- Product Marketing
---
