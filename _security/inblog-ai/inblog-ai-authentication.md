---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods described on the Inblog API and MCP Authentication page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Inblog Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inblog declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Inblog
provider_slug: inblog-ai
scheme_count: 2
schemes:
- evidence: Use an API key with the REST API, CLI, or AI Skills when you are running a script, integration, or coding workflow.
  how_to_obtain: Create it in Dashboard → Settings → API Keys .
  type: apiKey
- authorize_url: https://inblog.ai/api/mcp
  evidence: Use the MCP server when a person connects Inblog to Claude or ChatGPT at https://inblog.ai/api/mcp . The person signs in to Inblog and approves the connection through OAuth.
  flows:
  - authorization_code
  how_to_obtain: The person signs in to Inblog and approves the connection through OAuth.
  type: oauth2
slug: inblog-ai-authentication
source_filename: inblog-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://inblog.ai/docs/developer-tools/api-authentication
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://inblog.ai/docs/developer-tools/api-authentication\nsources:\n- https://inblog.ai/docs/developer-tools/api-authentication\n- https://inblog.ai/docs/seo-tutorial-domain-setup\n- https://inblog.ai/docs/start-inblog/getting-started-with-inblog\n- https://inblog.ai/docs/seo-tutorial-domain-setup/request-indexing\ndescription: Authentication methods described on the Inblog API and MCP Authentication page.\nschemes:\n- type: apiKey\n  evidence: Use an API key with the REST API, CLI, or AI Skills when you are running a script, integration, or coding workflow.\n  how_to_obtain: Create it in Dashboard → Settings → API Keys .\n- type: oauth2\n  evidence: Use the MCP server when a person connects Inblog to Claude or ChatGPT at https://inblog.ai/api/mcp . The person signs in to Inblog\n    and approves the connection through OAuth.\n  flows:\n  - authorization_code\n  authorize_url:\
  \ https://inblog.ai/api/mcp\n  how_to_obtain: The person signs in to Inblog and approves the connection through OAuth.\ndocs: https://inblog.ai/docs/developer-tools/api-authentication\n"
source_yaml_url: https://artifacts.apis.io/inblog-ai/authentication/inblog-ai-authentication.yml
summary_line: 2 schemes
tags:
- Blog Platform
- SEO
- AI Search
- No-Code
- Lead Capture
- Analytics
---
