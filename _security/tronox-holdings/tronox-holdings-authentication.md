---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Tronox Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tronox Holdings declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Tronox Holdings
provider_slug: tronox-holdings
scheme_count: 2
schemes:
- anonymous_response: 401 mcp_unauthorized ("MCP authentication required.")
  bearer_methods_supported:
  - header
  client_registration: No RFC 7591 dynamic client registration endpoint is advertised. The authorization server sets client_id_metadata_document_supported = true, so a client identifies itself with a URL to a client-id metadata document rather than a pre-registered client_id.
  discovery_chain: The 401 carries a WWW-Authenticate header whose resource_metadata parameter points at the RFC 9728 document, which names https://www.tronox.com as the authorization server, whose RFC 8414 document names the authorize/token/revoke endpoints - the full MCP authorization discovery chain works anonymously.
  evidence: https://www.tronox.com/.well-known/oauth-authorization-server/
  evidence_status: 200
  flows:
    authorizationCode:
      authorizationUrl: https://www.tronox.com/oauth/authorize
      refreshUrl: https://www.tronox.com/oauth/token
      revocationUrl: https://www.tronox.com/oauth/revoke
      scopes:
        mcp: Access the MCP server surface published by www.tronox.com
      tokenUrl: https://www.tronox.com/oauth/token
  id: mcp_oauth2
  pkce_required_methods:
  - S256
  surface: https://www.tronox.com/wp-json/mcp/mcp-oauth-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
  www_authenticate: Bearer realm="https://www.tronox.com", resource_metadata="https://www.tronox.com/.well-known/oauth-protected-resource"
- detail: Suppliers register and sign in with a Coupa Supplier Portal account and link it to Tronox; the FAQ on tronox.com covers registration, password reset and account merging inside Coupa. No Tronox credential, API key or integration token is described.
  evidence: https://www.tronox.com/supplier/coupa-supplier-portal/
  evidence_status: 200
  id: coupa_supplier_portal
  surface: Coupa Supplier Portal (third-party, supplier.coupahost.com)
  type: delegated
slug: tronox-holdings-authentication
source_filename: tronox-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: >-\n  https://www.tronox.com/.well-known/oauth-authorization-server/,\n  https://www.tronox.com/.well-known/oauth-protected-resource/,\n  https://www.tronox.com/supplier/coupa-supplier-portal/,\n  https://www.tronox.com/ethics-and-governance/data-privacy/\nsummary: >-\n  Tronox publishes no public REST API and therefore no OpenAPI securitySchemes. One\n  authentication surface is observable on a Tronox host: OAuth 2.0 (authorization code with\n  PKCE) in front of the MCP endpoint served by the WordPress MCP Adapter on www.tronox.com.\n  Supplier transactions (registration, sourcing events, purchase orders, ASNs, invoices) run on\n  the Coupa Supplier Portal, a third-party platform authenticated by Coupa's own accounts, not\n  by any Tronox-issued credential. Tronox does not issue a public API key.\n\nschemes:\n- id: mcp_oauth2\n  type: oauth2\n  surface: https://www.tronox.com/wp-json/mcp/mcp-oauth-server\n  flows:\n    authorizationCode:\n\
  \      authorizationUrl: https://www.tronox.com/oauth/authorize\n      tokenUrl: https://www.tronox.com/oauth/token\n      refreshUrl: https://www.tronox.com/oauth/token\n      revocationUrl: https://www.tronox.com/oauth/revoke\n      scopes:\n        mcp: Access the MCP server surface published by www.tronox.com\n  pkce_required_methods: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  client_registration: >-\n    No RFC 7591 dynamic client registration endpoint is advertised. The authorization server\n    sets client_id_metadata_document_supported = true, so a client identifies itself with a\n    URL to a client-id metadata document rather than a pre-registered client_id.\n  bearer_methods_supported: [header]\n  anonymous_response: 401 mcp_unauthorized (\"MCP authentication required.\")\n  www_authenticate: 'Bearer realm=\"https://www.tronox.com\", resource_metadata=\"https://www.tronox.com/.well-known/oauth-protected-resource\"'\n  discovery_chain: >-\n    The 401 carries\
  \ a WWW-Authenticate header whose resource_metadata parameter points at the\n    RFC 9728 document, which names https://www.tronox.com as the authorization server, whose\n    RFC 8414 document names the authorize/token/revoke endpoints - the full MCP authorization\n    discovery chain works anonymously.\n  evidence: https://www.tronox.com/.well-known/oauth-authorization-server/\n  evidence_status: 200\n\n- id: coupa_supplier_portal\n  type: delegated\n  surface: Coupa Supplier Portal (third-party, supplier.coupahost.com)\n  detail: >-\n    Suppliers register and sign in with a Coupa Supplier Portal account and link it to Tronox;\n    the FAQ on tronox.com covers registration, password reset and account merging inside\n    Coupa. No Tronox credential, API key or integration token is described.\n  evidence: https://www.tronox.com/supplier/coupa-supplier-portal/\n  evidence_status: 200\n\nnot_published:\n- api_keys: Tronox does not issue or document API keys.\n- openid_connect: /.well-known/openid-configuration\
  \ returns 404 on www.tronox.com.\n- sso_for_customers: no customer portal or customer login is published on tronox.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tronox-holdings/refs/heads/main/authentication/tronox-holdings-authentication.yml
summary_line: 2 schemes
tags:
- Titanium Dioxide
- Chemicals
- Mining
- Mineral Sands
- Zircon
- Pigments
- Manufacturing
---
