---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Laurel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Laurel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Laurel
provider_slug: checklaurel-com
scheme_count: 1
schemes:
- applies_to: https://checklaurel.com/mcp
  authorization_servers:
  - https://clerk.checklaurel.com
  bearer_methods_supported:
  - header
  evidence: '{"resource":"https://checklaurel.com/mcp","authorization_servers":["https://clerk.checklaurel.com"],"scopes_supported":["profile","email","offline_access"],"bearer_methods_supported":["header"],"resource_name":"Laurel"}'
  http_status: 200
  name: oauth2
  scopes:
  - profile
  - email
  - offline_access
  type: oauth2
slug: checklaurel-com-authentication
source_filename: checklaurel-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: https://checklaurel.com/.well-known/oauth-protected-resource\nsummary: The remote MCP server at https://checklaurel.com/mcp is an OAuth 2.0 protected resource (RFC 9728). Its\n  protected-resource metadata (HTTP 200) names https://clerk.checklaurel.com (Clerk-hosted) as the authorization server,\n  supports bearer tokens in the Authorization header only, and lists scopes profile, email and offline_access. No\n  OpenAPI or developer auth documentation is published; the Terms of Service require an account to use connectors.\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://checklaurel.com/mcp\n  authorization_servers:\n  - https://clerk.checklaurel.com\n  bearer_methods_supported:\n  - header\n  scopes:\n  - profile\n  - email\n  - offline_access\n  evidence: '{\"resource\":\"https://checklaurel.com/mcp\",\"authorization_servers\":[\"https://clerk.checklaurel.com\"],\"scopes_supported\":[\"profile\",\"email\",\"\
  offline_access\"],\"bearer_methods_supported\":[\"header\"],\"resource_name\":\"Laurel\"}'\n  http_status: 200\n"
source_yaml_url: https://artifacts.apis.io/checklaurel-com/authentication/checklaurel-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Consumer Products
- E-Commerce
- Product Discovery
- Low Tox
- Sustainability
- MCP
- Shopping
---
