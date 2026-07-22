---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Cumbuca Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cumbuca secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cumbuca
provider_slug: cumbuca
scheme_count: 3
schemes:
- description: 'The core regulated proxy forwards cryptographically signed, mutual-TLS requests between client infrastructure and the Bacen / Open Finance Brasil ecosystem using the client''s (or Cumbuca''s) certificates. Certificate swap when a client obtains its own Payment Institution license (zero lock-in).

    '
  name: OpenFinanceMTLS
  sources:
  - https://www.cumbuca.com/en/
  type: mutualTLS
- authorizationUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/auth
  description: 'The Open Finance Data MCP server is an OAuth 2.0 / OIDC protected resource. Authorization server is a Keycloak realm (idc.cumbuca.com/realms/cumbuca-mcp). Access tokens are mTLS certificate-bound (RFC 8705).

    '
  mtls_bound_tokens: true
  name: OpenIDConnect
  openIdConnectUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/.well-known/openid-configuration
  scopes_supported:
  - openid
  - profile
  - offline_access
  - open-finance
  sources:
  - https://mcp.cumbuca.com/.well-known/oauth-protected-resource
  tokenUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/token
  type: openIdConnect
- description: 'End-user data access follows the Open Finance Brasil consent flow: the user authenticates at their bank by CPF + biometric or banking PIN (no password sharing) and grants a scoped consent that Cumbuca relays.

    '
  name: OpenFinanceConsent
  sources:
  - https://www.cumbuca.com/en/launchweek/of-data-mcp/
  type: oauth2
slug: cumbuca-authentication
source_filename: cumbuca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource:\n  - https://mcp.cumbuca.com/.well-known/oauth-protected-resource\n  - https://idc.cumbuca.com/realms/cumbuca-mcp/.well-known/oauth-authorization-server\n  - https://www.cumbuca.com/en/\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\nschemes:\n  - name: OpenFinanceMTLS\n    type: mutualTLS\n    description: >\n      The core regulated proxy forwards cryptographically signed, mutual-TLS\n      requests between client infrastructure and the Bacen / Open Finance Brasil\n      ecosystem using the client's (or Cumbuca's) certificates. Certificate swap\n      when a client obtains its own Payment Institution license (zero lock-in).\n    sources: [https://www.cumbuca.com/en/]\n  - name: OpenIDConnect\n    type: openIdConnect\n    description: >\n      The Open Finance Data MCP server is an OAuth 2.0 / OIDC protected resource.\n      Authorization server is a Keycloak realm\
  \ (idc.cumbuca.com/realms/cumbuca-mcp).\n      Access tokens are mTLS certificate-bound (RFC 8705).\n    openIdConnectUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/.well-known/openid-configuration\n    authorizationUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/auth\n    tokenUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/token\n    scopes_supported: [openid, profile, offline_access, open-finance]\n    mtls_bound_tokens: true\n    sources: [https://mcp.cumbuca.com/.well-known/oauth-protected-resource]\n  - name: OpenFinanceConsent\n    type: oauth2\n    description: >\n      End-user data access follows the Open Finance Brasil consent flow: the user\n      authenticates at their bank by CPF + biometric or banking PIN (no password\n      sharing) and grants a scoped consent that Cumbuca relays.\n    sources: [https://www.cumbuca.com/en/launchweek/of-data-mcp/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cumbuca/refs/heads/main/authentication/cumbuca-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Company
- Fintech
- Open Finance
- Pix
- Payments
- Banking
- Brazil
- Open Banking
- Financial Data
- MCP
---
