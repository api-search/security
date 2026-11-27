---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CrawlRaven Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrawlRaven declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CrawlRaven
provider_slug: crawlraven-com
scheme_count: 1
schemes:
- access_token_lifetime: 1 hour
  applies_to: https://mcp.crawlraven.com/mcp
  description: 'Authorization: OAuth authorization code with S256 PKCE'
  dynamic_client_registration: true
  flow: authorizationCode
  name: crawlraven-mcp-oauth
  pkce: S256
  redirect_rules: HTTPS callbacks match exactly; native clients may use HTTP loopback callbacks. Cursor may use its exact application-owned callback; other private-use schemes are rejected.
  refresh_token_lifetime: 'Grant, refresh token, and DCR registration expiry: 90 days'
  scopes_ref: scopes/crawlraven-com-scopes.yml
  type: oauth2
slug: crawlraven-com-authentication
source_filename: crawlraven-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://crawlraven.com/docs/mcp\ndocs: https://crawlraven.com/docs/mcp\nnote: No OpenAPI contract exists; CrawlRaven's docs state no public REST API is offered in v2. This profile covers the remote MCP server only, as documented.\nschemes:\n- name: crawlraven-mcp-oauth\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  applies_to: https://mcp.crawlraven.com/mcp\n  description: \"Authorization: OAuth authorization code with S256 PKCE\"\n  access_token_lifetime: 1 hour\n  refresh_token_lifetime: \"Grant, refresh token, and DCR registration expiry: 90 days\"\n  dynamic_client_registration: true\n  redirect_rules: \"HTTPS callbacks match exactly; native clients may use HTTP loopback callbacks. Cursor may use its exact application-owned callback; other private-use schemes are rejected.\"\n  scopes_ref: scopes/crawlraven-com-scopes.yml\napi_keys: \"There are no API keys to create or paste. (https://crawlraven.com/changelog)\"\
  \n"
source_yaml_url: https://artifacts.apis.io/crawlraven-com/authentication/crawlraven-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- SEO
- Search Console
- Google Analytics
- Technical SEO Audit
- Analytics
- MCP
- Marketing
---
