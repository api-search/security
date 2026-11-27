---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cookiefreeanalytics-com-sites-api-openapi.yml
  format: yaml
  label: Cookie Free Analytics Sites API
  slug: cookiefreeanalytics-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiefreeanalytics-com/openapi/cookiefreeanalytics-com-sites-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cookie Free Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cookie Free Analytics secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cookie Free Analytics
provider_slug: cookiefreeanalytics-com
scheme_count: 2
schemes:
- applies_to: Read API (/api/v1) and the /mcp endpoint
  bearerFormat: cfa_live_
  description: 'Plan → Account → Read API → name a token. We show cfa_live_… once. We store a hash. Send it as Authorization: Bearer . Revoke on the same page. Read API tokens are available on Starter and Growth.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/cookiefreeanalytics-com-openapi.yml
  - https://www.cookiefreeanalytics.com/docs/api
  type: http
- applies_to: https://www.cookiefreeanalytics.com/mcp
  authorization_servers:
  - https://www.cookiefreeanalytics.com
  bearer_methods_supported:
  - header
  description: Claude, Cursor, ChatGPT, and Grok use OAuth 2.1 on this host (RFC 9728 metadata, PKCE S256). The client discovers OAuth and opens /oauth/authorize. Hobby (free) gets 5 MCP tools through OAuth.
  name: mcp-oauth
  pkce: S256
  protected_resource_metadata: https://www.cookiefreeanalytics.com/.well-known/oauth-protected-resource
  scopes_supported:
  - analytics:read
  - sites:write
  sources:
  - https://www.cookiefreeanalytics.com/docs/api
  - https://www.cookiefreeanalytics.com/.well-known/oauth-protected-resource
  type: oauth2
slug: cookiefreeanalytics-com-authentication
source_filename: cookiefreeanalytics-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.cookiefreeanalytics.com/docs/api\ndocs: https://www.cookiefreeanalytics.com/docs/api\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: cfa_live_\n  applies_to: Read API (/api/v1) and the /mcp endpoint\n  description: 'Plan → Account → Read API → name a token. We show cfa_live_… once. We store a hash. Send it as Authorization: Bearer . Revoke on the same page. Read API tokens are available on Starter and Growth.'\n  sources:\n  - openapi/cookiefreeanalytics-com-openapi.yml\n  - https://www.cookiefreeanalytics.com/docs/api\n- name: mcp-oauth\n  type: oauth2\n  applies_to: https://www.cookiefreeanalytics.com/mcp\n  description: Claude, Cursor, ChatGPT, and Grok use OAuth 2.1 on this host (RFC 9728 metadata, PKCE S256). The client discovers OAuth and opens /oauth/authorize. Hobby (free) gets 5 MCP tools through OAuth.\n  protected_resource_metadata:\
  \ https://www.cookiefreeanalytics.com/.well-known/oauth-protected-resource\n  authorization_servers:\n  - https://www.cookiefreeanalytics.com\n  bearer_methods_supported:\n  - header\n  scopes_supported:\n  - analytics:read\n  - sites:write\n  pkce: S256\n  sources:\n  - https://www.cookiefreeanalytics.com/docs/api\n  - https://www.cookiefreeanalytics.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/cookiefreeanalytics-com/authentication/cookiefreeanalytics-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Analytics
- Web Analytics
- Privacy
- Cookieless
- GDPR
- MCP
- Uptime Monitoring
---
