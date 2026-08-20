---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- none
description: ''
kind: authentication
layout: security
method: searched
name: Beekeepers Naturals Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Beekeeper's Naturals secures its APIs with openIdConnect, oauth2, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Beekeeper's Naturals
provider_slug: beekeepers-naturals
scheme_count: 3
schemes:
- authorizationUrl: https://account.beekeepersnaturals.com/authentication/oauth/authorize
  codeChallengeMethods:
  - S256
  endSessionUrl: https://account.beekeepersnaturals.com/authentication/logout
  grantTypes:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  idTokenSigningAlgs:
  - RS256
  issuer: https://shopify.com/authentication/2905473113
  jwksUri: https://account.beekeepersnaturals.com/authentication/.well-known/jwks.json
  name: shopify-customer-accounts
  openIdConnectUrl: https://www.beekeepersnaturals.com/.well-known/openid-configuration
  responseTypes:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/beekeepers-naturals-openid-configuration.json
  - well-known/beekeepers-naturals-oauth-authorization-server.json
  tokenEndpointAuthMethods:
  - client_secret_basic
  tokenUrl: https://account.beekeepersnaturals.com/authentication/oauth/token
  type: openIdConnect
- description: Every call to the UCP Shopping MCP endpoint must identify the calling platform with a resolvable URI pointing at that platform's UCP profile document. This is agent identification, not buyer authentication — an anonymous call is rejected with JSON-RPC -32001 / invalid_profile_url.
  in: header
  json_rpc_path: params.meta["ucp-agent"].profile
  name: ucp-agent-profile
  parameter: UCP-Agent
  required: true
  sources:
  - https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json
  - mcp/beekeepers-naturals-mcp.yml
  type: agentIdentity
- description: Read-only storefront product and collection JSON requires no authentication.
  name: storefront-public
  sources:
  - https://www.beekeepersnaturals.com/agents.md
  type: none
slug: beekeepers-naturals-authentication
source_filename: beekeepers-naturals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://www.beekeepersnaturals.com/.well-known/openid-configuration\ndocs: https://www.beekeepersnaturals.com/agents.md\nnote: 'No OpenAPI exists for this provider, so this profile is built from live discovery documents fetched\n  from the store''s own hosts, not derived from a spec.'\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - none\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  api_key_in: []\nschemes:\n- name: shopify-customer-accounts\n  type: openIdConnect\n  openIdConnectUrl: https://www.beekeepersnaturals.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/2905473113\n  authorizationUrl: https://account.beekeepersnaturals.com/authentication/oauth/authorize\n  tokenUrl: https://account.beekeepersnaturals.com/authentication/oauth/token\n  endSessionUrl: https://account.beekeepersnaturals.com/authentication/logout\n  jwksUri: https://account.beekeepersnaturals.com/authentication/.well-known/jwks.json\n\
  \  responseTypes: [code]\n  grantTypes:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  tokenEndpointAuthMethods: [client_secret_basic]\n  codeChallengeMethods: [S256]\n  idTokenSigningAlgs: [RS256]\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/beekeepers-naturals-openid-configuration.json\n  - well-known/beekeepers-naturals-oauth-authorization-server.json\n- name: ucp-agent-profile\n  type: agentIdentity\n  in: header\n  parameter: UCP-Agent\n  json_rpc_path: params.meta[\"ucp-agent\"].profile\n  description: 'Every call to the UCP Shopping MCP endpoint must identify the calling platform with a\n    resolvable URI pointing at that platform''s UCP profile document. This is agent identification, not\n    buyer authentication — an anonymous call is rejected with JSON-RPC -32001 / invalid_profile_url.'\n  required: true\n  sources:\n  - https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json\n\
  \  - mcp/beekeepers-naturals-mcp.yml\n- name: storefront-public\n  type: none\n  description: Read-only storefront product and collection JSON requires no authentication.\n  sources:\n  - https://www.beekeepersnaturals.com/agents.md\nprotected_resource:\n  resource: https://www.beekeepersnaturals.com\n  authorization_servers:\n  - https://account.beekeepersnaturals.com\n  - https://shopify.com/authentication/2905473113\n  bearer_methods_supported: [header]\n  source: well-known/beekeepers-naturals-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - {url: 'https://www.beekeepersnaturals.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://www.beekeepersnaturals.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://www.beekeepersnaturals.com/.well-known/oauth-protected-resource', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beekeepers-naturals/refs/heads/main/authentication/beekeepers-naturals-authentication.yml
summary_line: openIdConnect/oauth2/none · 3 schemes
tags:
- Company
- Retail
- E-Commerce
- Consumer Packaged Goods
- Health and Wellness
- Supplements
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
---
