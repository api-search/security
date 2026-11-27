---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chimpanseo-app-audit-api-openapi.yml
  format: yaml
  label: ChimpanSEO Audit API
  slug: chimpanseo-app-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimpanseo-app/openapi/chimpanseo-app-audit-api-openapi.yml
- filename: chimpanseo-app-mcp-api-openapi.yml
  format: yaml
  label: ChimpanSEO MCP API
  slug: chimpanseo-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimpanseo-app/openapi/chimpanseo-app-mcp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ChimpanSEO Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChimpanSEO declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ChimpanSEO
provider_slug: chimpanseo-app
scheme_count: 2
schemes:
- description: API key created in the dashboard (Settings > API/MCP). Keys start with csk_ and can be full access or read-only.
  header: 'Authorization: Bearer <API key>'
  name: bearerApiKey
  scheme: bearer
  type: http
- description: Same API key sent as x-api-key header.
  header_name: x-api-key
  in: header
  name: headerApiKey
  type: apiKey
slug: chimpanseo-app-authentication
source_filename: chimpanseo-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chimpanseo.app/mcp\ndocs: https://chimpanseo.app/mcp\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <API key>'\n  description: API key created in the dashboard (Settings > API/MCP). Keys start with csk_ and can be full access or read-only.\n- name: headerApiKey\n  type: apiKey\n  in: header\n  header_name: x-api-key\n  description: Same API key sent as x-api-key header.\nkey_prefix: csk_\nkey_types:\n- name: full access\n  description: Required for write tools (generate_article, refresh_article, publish_article, schedule_article, cancel_scheduled_article).\n- name: read-only\n  description: Can list sites, articles and the calendar, read articles, suggest topics and run audits, but cannot generate, refresh, publish or schedule.\nanonymous: initialize, ping, tools/list, resources/list and prompts/list on the MCP endpoint work without a key; tools/call requires a key.\
  \ Public audit endpoints need no key.\noauth: 'Not supported: \"Does it support OAuth? Not yet.\"'\n"
source_yaml_url: https://artifacts.apis.io/chimpanseo-app/authentication/chimpanseo-app-authentication.yml
summary_line: 2 schemes
tags:
- Company
- SEO
- Generative Engine Optimization
- AI Content
- Content Marketing
- WordPress
- MCP
---
