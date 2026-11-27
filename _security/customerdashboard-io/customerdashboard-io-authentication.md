---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CustomerDashboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: CustomerDashboard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CustomerDashboard
provider_slug: customerdashboard-io
scheme_count: 1
schemes:
- applies_to: https://app.customerdashboard.io/mcp
  bearer_methods:
  - header
  client_auth: none
  dynamic_client_registration: https://app.customerdashboard.io/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://app.customerdashboard.io/oauth/authorize
      refresh: true
      tokenUrl: https://app.customerdashboard.io/oauth/token
  name: oauth2
  pkce: S256
  scopes:
  - account:read
  - dashboards:read
  - dashboards:write
  - datasources:read
  - datasources:write
  - data:read
  - customers:read
  - customers:write
  - publish
  - delete
  type: oauth2
slug: customerdashboard-io-authentication
source_filename: customerdashboard-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://app.customerdashboard.io/docs/mcp/\ndocs: https://app.customerdashboard.io/docs/mcp/\nsummary: The MCP server at https://app.customerdashboard.io/mcp uses OAuth 2.0 authorization code with PKCE (S256), public clients (token_endpoint_auth_method none) and dynamic client registration. Docs state \"You do not create a static API token. The client starts OAuth, you sign in with the same account you use on the website (Google or email)\". A tool call that needs an account and arrives without a token gets 401 plus a WWW-Authenticate challenge. No REST API or API keys are published.\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://app.customerdashboard.io/mcp\n  bearer_methods: [header]\n  flows:\n    authorizationCode:\n      authorizationUrl: https://app.customerdashboard.io/oauth/authorize\n      tokenUrl: https://app.customerdashboard.io/oauth/token\n      refresh: true\n  pkce: S256\n  client_auth: none\n\
  \  dynamic_client_registration: https://app.customerdashboard.io/oauth/register\n  scopes: [account:read, dashboards:read, dashboards:write, datasources:read, datasources:write, data:read, customers:read, customers:write, publish, delete]\ndiscovery:\n- url: https://app.customerdashboard.io/.well-known/oauth-protected-resource/mcp\n  http_status: 200\n  standard: RFC 9728\n- url: https://app.customerdashboard.io/.well-known/oauth-authorization-server\n  http_status: 200\n  standard: RFC 8414\nunauthenticated_tools: [get_platform_overview, list_supported_data_connectors, list_widget_types, list_plans_and_limits, explain_customer_filtering, get_started]\n"
source_yaml_url: https://artifacts.apis.io/customerdashboard-io/authentication/customerdashboard-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Analytics
- Dashboards
- Customer-Facing Analytics
- Embedded Analytics
- Client Reporting
- White Label
- Multi-Tenant
- MCP
- Software-as-a-Service
---
