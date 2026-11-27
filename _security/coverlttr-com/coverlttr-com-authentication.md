---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coverlttr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coverlttr declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Coverlttr
provider_slug: coverlttr-com
scheme_count: 1
schemes:
- applies_to: https://mcp.coverlttr.com
  authorization_servers:
  - https://www.coverlttr.com
  bearer_methods_supported:
  - header
  evidence:
  - http_status: 200
    url: https://www.coverlttr.com/mcp.md
  - http_status: 200
    url: https://mcp.coverlttr.com/.well-known/oauth-protected-resource
  flow: authorizationCode (browser sign-in on first connection)
  name: oauth2
  quote: 'Authentication**: OAuth 2.1 (browser sign-in on first connection; no manual API keys required)'
  scopes:
  - coverlttr:read
  - coverlttr:write
  type: oauth2
  version: OAuth 2.1
slug: coverlttr-com-authentication
source_filename: coverlttr-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.coverlttr.com/mcp.md\ndocs: https://www.coverlttr.com/mcp\nsummary: The only published programmatic surface is the remote MCP server at https://mcp.coverlttr.com (ChatGPT uses https://mcp.coverlttr.com/chatgpt/mcp). The docs say it uses OAuth 2.1 with browser sign-in on first connection and no API keys. Its OAuth protected-resource metadata (GET https://mcp.coverlttr.com/.well-known/oauth-protected-resource, HTTP 200) names https://www.coverlttr.com as the authorization server and accepts bearer tokens in the header only. No OpenAPI contract is published.\nschemes:\n- name: oauth2\n  type: oauth2\n  version: OAuth 2.1\n  flow: authorizationCode (browser sign-in on first connection)\n  bearer_methods_supported: [header]\n  authorization_servers: [https://www.coverlttr.com]\n  scopes: [coverlttr:read, coverlttr:write]\n  applies_to: https://mcp.coverlttr.com\n  quote: \"Authentication**: OAuth 2.1 (browser sign-in\
  \ on first connection; no manual API keys required)\"\n  evidence:\n  - url: https://www.coverlttr.com/mcp.md\n    http_status: 200\n  - url: https://mcp.coverlttr.com/.well-known/oauth-protected-resource\n    http_status: 200\napi_keys: none\napi_keys_note: The FAQ says \"Coverlttr never asks you to paste long-lived API keys into chat.\" No API-key scheme is documented.\n"
source_yaml_url: https://artifacts.apis.io/coverlttr-com/authentication/coverlttr-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Cover Letters
- Job Search
- Careers
- Artificial Intelligence
- Writing
- MCP
---
