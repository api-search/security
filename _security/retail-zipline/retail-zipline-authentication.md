---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Retail Zipline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Retail Zipline declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Retail Zipline
provider_slug: retail-zipline
scheme_count: 1
schemes:
- applies_to: https://getzipline.com/wp-json/mcp/mcp-oauth-server
  authorization_response_iss_parameter_supported: true
  bearer_methods_supported:
  - header
  client_registration: client_id_metadata_document_supported = true — clients identify themselves by a URL-addressable client ID metadata document rather than pre-registering.
  flows:
    authorizationCode:
      authorizationUrl: https://getzipline.com/oauth/authorize
      refreshUrl: https://getzipline.com/oauth/token
      scopes:
        mcp: Access the Zipline MCP server
      tokenUrl: https://getzipline.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  key: oauth2_mcp
  notes: 'Public client profile: token_endpoint_auth_methods_supported is ["none"], so no client secret is used; PKCE S256 is the protection. This is the OAuth 2.1 / MCP authorization profile.'
  pkce_methods:
  - S256
  pkce_required: true
  response_types_supported:
  - code
  revocation_endpoint: https://getzipline.com/oauth/revoke
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: retail-zipline-authentication
source_filename: retail-zipline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://getzipline.com/.well-known/oauth-authorization-server\nsummary: >-\n  Zipline publishes no public developer authentication documentation. The only\n  machine-readable auth description it serves is RFC 8414 OAuth Authorization\n  Server Metadata on getzipline.com, which governs its MCP endpoint. Access to\n  the Zipline retail operations product itself is via customer SSO on a\n  per-tenant subdomain and is not publicly documented.\nschemes:\n- key: oauth2_mcp\n  type: oauth2\n  applies_to: https://getzipline.com/wp-json/mcp/mcp-oauth-server\n  flows:\n    authorizationCode:\n      authorizationUrl: https://getzipline.com/oauth/authorize\n      tokenUrl: https://getzipline.com/oauth/token\n      refreshUrl: https://getzipline.com/oauth/token\n      scopes:\n        mcp: Access the Zipline MCP server\n  pkce_required: true\n  pkce_methods:\n  - S256\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n\
  \  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  bearer_methods_supported:\n  - header\n  revocation_endpoint: https://getzipline.com/oauth/revoke\n  client_registration: >-\n    client_id_metadata_document_supported = true — clients identify themselves by\n    a URL-addressable client ID metadata document rather than pre-registering.\n  authorization_response_iss_parameter_supported: true\n  notes: >-\n    Public client profile: token_endpoint_auth_methods_supported is [\"none\"], so\n    no client secret is used; PKCE S256 is the protection. This is the OAuth 2.1\n    / MCP authorization profile.\nend_user_authentication:\n  product: Zipline retail operations platform\n  host_pattern: https://<customer>.retailzipline.com\n  methods:\n  - SAML / SSO (an Okta application integration for Retail Zipline is published in the Okta Integration Network)\n  - Username + password with password reset\n  - Biometric login on mobile (iOS/Android apps)\n  documented_publicly:\
  \ false\n  note: >-\n    No public API key, token or developer-credential documentation was found on\n    any Zipline-controlled host. Product authentication detail is customer-facing\n    only.\nx-evidence:\n- url: https://getzipline.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-26'\n- url: https://www.okta.com/integrations/retail-zipline/\n  http_status: 200\n  note: third-party confirmation of SAML/SSO support\n  fetched: '2026-08-26'\n- url: https://support.retailzipline.com/en/articles/16299801-biometric-login-supported-devices-and-troubleshooting\n  http_status: 200\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retail-zipline/refs/heads/main/authentication/retail-zipline-authentication.yml
summary_line: 1 scheme
tags:
- Retail
- Retail Operations
- Task Management
- Employee Communications
- Store Operations
- Workforce
- Knowledge Base
- Software-as-a-Service
- MCP
- Company
---
