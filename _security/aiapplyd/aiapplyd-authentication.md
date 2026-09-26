---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aiapplyd-openapi.yml
  format: yaml
  label: AI Applyd API
  slug: ai-applyd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aiapplyd/refs/heads/main/openapi/aiapplyd-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Aiapplyd Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Applyd declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AI Applyd
provider_slug: aiapplyd
scheme_count: 3
schemes:
- applies_to: AI Applyd API (api.aiapplyd.com/api/v1)
  description: 'Session token from signing in to AI Applyd, sent as `Authorization: Bearer <token>` (the contract''s own components.securitySchemes.BearerAuth description).'
  name: BearerAuth
  note: Declared in components.securitySchemes and applied as the top-level security requirement since the 2026-09-25 contract; on 2026-09-23 it was referenced but undeclared.
  scheme: bearer
  type: http
- applies_to: internal service-to-service route /mcp/session (the /internal/* routes left the public contract on 2026-09-25)
  description: Operation descriptions say "Internal (x-api-key)".
  in: header
  name: x-api-key
  type: apiKey
- applies_to: AI Applyd MCP Server (mcp.aiapplyd.com/mcp)
  authorization_response_iss_parameter_supported: true
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.aiapplyd.com/authorize
      refreshUrl: https://mcp.aiapplyd.com/oauth/token
      tokenUrl: https://mcp.aiapplyd.com/oauth/token
  name: MCP OAuth
  pkce: S256
  registration_endpoint: https://mcp.aiapplyd.com/register
  revocation_endpoint: https://mcp.aiapplyd.com/oauth/revoke
  scopes:
  - openid
  - email
  - profile
  - offline_access
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: aiapplyd-authentication
source_filename: aiapplyd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: searched\nsource:\n- https://api.aiapplyd.com/api/v1/openapi.json\n- https://mcp.aiapplyd.com/.well-known/oauth-authorization-server\n- https://mcp.aiapplyd.com/.well-known/oauth-protected-resource\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  applies_to: AI Applyd API (api.aiapplyd.com/api/v1)\n  description: 'Session token from signing in to AI Applyd, sent as `Authorization: Bearer <token>` (the contract''s own components.securitySchemes.BearerAuth\n    description).'\n  note: Declared in components.securitySchemes and applied as the top-level security requirement since the 2026-09-25 contract;\n    on 2026-09-23 it was referenced but undeclared.\n- name: x-api-key\n  type: apiKey\n  in: header\n  applies_to: internal service-to-service route /mcp/session (the /internal/* routes left the public contract on 2026-09-25)\n  description: Operation descriptions say \"Internal (x-api-key)\".\n- name: MCP OAuth\n  type: oauth2\n\
  \  applies_to: AI Applyd MCP Server (mcp.aiapplyd.com/mcp)\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.aiapplyd.com/authorize\n      tokenUrl: https://mcp.aiapplyd.com/oauth/token\n      refreshUrl: https://mcp.aiapplyd.com/oauth/token\n  pkce: S256\n  registration_endpoint: https://mcp.aiapplyd.com/register\n  revocation_endpoint: https://mcp.aiapplyd.com/oauth/revoke\n  token_endpoint_auth_methods:\n  - none\n  bearer_methods:\n  - header\n  scopes:\n  - openid\n  - email\n  - profile\n  - offline_access\n  client_id_metadata_document_supported: true\n  authorization_response_iss_parameter_supported: true\nsummary: REST backend uses session bearer tokens (BearerAuth, declared in the contract); the MCP server is an OAuth 2.1 protected\n  resource (RFC 9728) with public clients, PKCE, dynamic client registration, Client ID Metadata Documents and the RFC 9207\n  iss parameter.\ndocs: https://aiapplyd.com/mcps\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiapplyd/refs/heads/main/authentication/aiapplyd-authentication.yml
summary_line: 3 schemes
tags:
- Job Search
- Recruiting
- Resume
- Applicant Tracking Systems
- Careers
- Artificial Intelligence
- MCP
- Automation
---
