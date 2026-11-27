---
anonymous_access: false
api_key_in: []
api_specs:
- filename: defoorreport-com-news-api-openapi.yml
  format: yaml
  label: DeFoor Report News API
  slug: defoorreport-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defoorreport-com/openapi/defoorreport-com-news-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: DeFoor Report Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeFoor Report secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DeFoor Report
provider_slug: defoorreport-com
scheme_count: 2
schemes:
- applies_to: News API (GET https://argolabs.us/v1/news)
  description: Your DeFoor Report key (starts with ts_live_).
  header: 'Authorization: Bearer <your key>'
  key_prefix: ts_live_
  name: bearerKey
  obtain: Free key emailed after confirming an email address at https://defoorreport.com/subscribe ("Add the Report to your AI").
  scheme: bearer
  sources:
  - openapi/defoorreport-com-openapi.yml
  - https://defoorreport.com/llms.txt
  - https://defoorreport.com/subscribe
  type: http
- applies_to: MCP server
  description: The MCP server at https://mcp.defoorreport.com/mcp uses "OAuth sign-in with the reader's DeFoor Report email" (llms.txt). Flows, endpoints and scopes are not published in the docs read here; not probed (auth endpoints are out of bounds).
  name: mcpOAuth
  sources:
  - https://defoorreport.com/llms.txt
  type: oauth2
slug: defoorreport-com-authentication
source_filename: defoorreport-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://defoorreport.com/llms.txt\ndocs: https://defoorreport.com/subscribe\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerKey\n  type: http\n  scheme: bearer\n  description: Your DeFoor Report key (starts with ts_live_).\n  header: 'Authorization: Bearer <your key>'\n  key_prefix: ts_live_\n  obtain: Free key emailed after confirming an email address at https://defoorreport.com/subscribe (\"Add the Report to your AI\").\n  applies_to: News API (GET https://argolabs.us/v1/news)\n  sources:\n  - openapi/defoorreport-com-openapi.yml\n  - https://defoorreport.com/llms.txt\n  - https://defoorreport.com/subscribe\n- name: mcpOAuth\n  type: oauth2\n  description: The MCP server at https://mcp.defoorreport.com/mcp uses \"OAuth sign-in with the reader's DeFoor Report email\" (llms.txt). Flows, endpoints and scopes are not published in the docs read here; not probed (auth endpoints are out of bounds).\n  applies_to:\
  \ MCP server\n  sources:\n  - https://defoorreport.com/llms.txt\n"
source_yaml_url: https://artifacts.apis.io/defoorreport-com/authentication/defoorreport-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- News
- Artificial Intelligence
- Media
- News Aggregation
- MCP
- LLM
---
