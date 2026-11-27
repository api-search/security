---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CounselAudit Authentication
name_suffix: Authentication
oauth_flows: []
overview: CounselAudit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CounselAudit
provider_slug: counselaudit-com
scheme_count: 1
schemes:
- applies_to: CounselAudit MCP Connector (https://app.counselaudit.com/api/mcp/mcp)
  authorization_server: https://clerk.counselaudit.com
  authorization_server_metadata: https://clerk.counselaudit.com/.well-known/oauth-authorization-server
  description: Authenticate with your existing CounselAudit login over OAuth 2.1. Access is scoped to your organization and enforced at the database layer.
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  name: oauth2
  pkce: S256
  protected_resource_metadata: https://app.counselaudit.com/.well-known/oauth-protected-resource/mcp
  token_endpoint_auth_methods:
  - client_secret_basic
  - none
  - client_secret_post
  token_location: header
  type: oauth2
slug: counselaudit-com-authentication
source_filename: counselaudit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.counselaudit.com/mcp.html\ndocs: https://www.counselaudit.com/mcp.html\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: CounselAudit MCP Connector (https://app.counselaudit.com/api/mcp/mcp)\n  description: Authenticate with your existing CounselAudit login over OAuth 2.1. Access is scoped to your organization and enforced at the database layer.\n  authorization_server: https://clerk.counselaudit.com\n  protected_resource_metadata: https://app.counselaudit.com/.well-known/oauth-protected-resource/mcp\n  authorization_server_metadata: https://clerk.counselaudit.com/.well-known/oauth-authorization-server\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:device_code']\n  pkce: S256\n  dynamic_client_registration: true\n  token_endpoint_auth_methods: [client_secret_basic, none, client_secret_post]\n  token_location: header\napi_keys: false\nnote: The docs state \"One URL, no\
  \ API keys to copy around.\" Grant types, PKCE and registration support were read (GET only) from the published RFC 9728 / RFC 8414 metadata documents; the MCP endpoint itself answers 401 invalid_token anonymously. No REST API exists.\n"
source_yaml_url: https://artifacts.apis.io/counselaudit-com/authentication/counselaudit-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Legal Tech
- Legal Billing
- Invoice Review
- E-Billing
- Outside Counsel Guidelines
- Artificial Intelligence
- MCP
---
