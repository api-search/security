---
anonymous_access: true
api_key_in: []
api_specs:
- filename: crawlconsole-com-agentic-commerce-api-openapi.yml
  format: yaml
  label: CrawlConsole Agentic commerce API
  slug: crawlconsole-com-agentic-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlconsole-com/openapi/crawlconsole-com-agentic-commerce-api-openapi.yml
- filename: crawlconsole-com-backlinks-api-openapi.yml
  format: yaml
  label: CrawlConsole Backlinks API
  slug: crawlconsole-com-backlinks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlconsole-com/openapi/crawlconsole-com-backlinks-api-openapi.yml
- filename: crawlconsole-com-webmcp-api-openapi.yml
  format: yaml
  label: CrawlConsole Web MCP API
  slug: crawlconsole-com-webmcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlconsole-com/openapi/crawlconsole-com-webmcp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CrawlConsole Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrawlConsole declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CrawlConsole
provider_slug: crawlconsole-com
scheme_count: 3
schemes:
- applies_to: Remote MCP server https://crawlconsole.com/mcp
  description: 'Create a key in Settings > API Keys; send as "Authorization: Bearer YOUR_AGENT_API_KEY". Raw secret shown once; keys carry scopes and optional domain restrictions and can be revoked independently.'
  name: Agent API key (bearer)
  scheme: bearer
  type: http
- applies_to: Remote MCP server
  description: OAuth discovery is also available from CrawlConsole's well-known authorization metadata for clients that support the remote authorization flow.
  name: OAuth remote authorization
  type: oauth2
- applies_to: getDomainScore, checkWebMcpReadiness, checkUcpReadiness (public checkers)
  name: none
  type: none
slug: crawlconsole-com-authentication
source_filename: crawlconsole-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://crawlconsole.com/docs/agents/mcp\ndocs: https://crawlconsole.com/docs/agents/mcp\nnote: 'The three public checker operations in the OpenAPI declare no security. The docs say \"Authenticated product and Agent APIs use their own session or bearer-token requirements.\"'\nschemes:\n- name: Agent API key (bearer)\n  type: http\n  scheme: bearer\n  applies_to: Remote MCP server https://crawlconsole.com/mcp\n  description: 'Create a key in Settings > API Keys; send as \"Authorization: Bearer YOUR_AGENT_API_KEY\". Raw secret shown once; keys carry scopes and optional domain restrictions and can be revoked independently.'\n- name: OAuth remote authorization\n  type: oauth2\n  applies_to: Remote MCP server\n  description: OAuth discovery is also available from CrawlConsole's well-known authorization metadata for clients that support the remote authorization flow.\n- name: none\n  type: none\n  applies_to: getDomainScore, checkWebMcpReadiness,\
  \ checkUcpReadiness (public checkers)\n"
source_yaml_url: https://artifacts.apis.io/crawlconsole-com/authentication/crawlconsole-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI Agents
- Analytics
- SEO
- Web Crawlers
- Backlinks
- MCP
- WebMCP
---
