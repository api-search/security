---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Clootrack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clootrack declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clootrack
provider_slug: clootrack-com
scheme_count: 1
schemes:
- applies_to: https://mcp.clootrack.com
  client_id_metadata_document_supported: true
  dynamic_client_registration: https://mcp.clootrack.com/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.clootrack.com/oauth/authorize
      refreshUrl: https://mcp.clootrack.com/oauth/token
      scopes:
      - openid
      - profile
      - offline_access
      tokenUrl: https://mcp.clootrack.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.clootrack.com
  name: clootrack-mcp-oauth2
  pkce: S256
  protected_resource_metadata: https://mcp.clootrack.com/.well-known/oauth-protected-resource
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: clootrack-com-authentication
source_filename: clootrack-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://mcp.clootrack.com/.well-known/oauth-authorization-server\ndocs: https://www.clootrack.com/mcp\nsummary: >-\n  Clootrack publishes no REST/OpenAPI contract. Its only advertised programmatic surface is the remote MCP server\n  at https://mcp.clootrack.com (official MCP registry entry com.clootrack/mcp, streamable-http). That server publishes\n  RFC 9728 protected-resource metadata and RFC 8414 authorization-server metadata (both HTTP 200, read 2026-11-04):\n  OAuth 2.0 authorization code with PKCE (S256), public clients (token_endpoint_auth_methods_supported: none),\n  dynamic client registration and client ID metadata documents. Clootrack's MCP page states access follows the\n  role-based access controls configured in the Clootrack platform. Token/authorize/register endpoints were read\n  from metadata only and were not called.\nschemes:\n- name: clootrack-mcp-oauth2\n  type: oauth2\n  applies_to: https://mcp.clootrack.com\n\
  \  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.clootrack.com/oauth/authorize\n      tokenUrl: https://mcp.clootrack.com/oauth/token\n      refreshUrl: https://mcp.clootrack.com/oauth/token\n      scopes: [openid, profile, offline_access]\n  pkce: S256\n  token_endpoint_auth_methods: [none]\n  grant_types: [authorization_code, refresh_token]\n  dynamic_client_registration: https://mcp.clootrack.com/oauth/register\n  client_id_metadata_document_supported: true\n  protected_resource_metadata: https://mcp.clootrack.com/.well-known/oauth-protected-resource\n  issuer: https://mcp.clootrack.com\n"
source_yaml_url: https://artifacts.apis.io/clootrack-com/authentication/clootrack-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Customer Experience
- Voice of the Customer
- Customer Feedback Analytics
- Artificial Intelligence
- Sentiment Analysis
- MCP
---
