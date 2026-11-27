---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Controlflare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Controlflare declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Controlflare
provider_slug: controlflare-com
scheme_count: 2
schemes:
- applies_to: https://app.controlflare.com/mcp
  description: OAuth 2.1 for the remote MCP server. A first call to /mcp returns 401 with a WWW-Authenticate header naming the protected-resource metadata. The client then registers itself (dynamic client registration) and opens a consent page that names the client and lists what it can do. The user then signs in with Cloudflare.
  name: mcp-oauth
  quote: A first call to /mcp comes back 401 with a WWW-Authenticate header naming the protected-resource metadata; the client reads that, registers itself, and opens the consent page in your browser.
  revocation: Remove the connection in the client. The next call gets a 401.
  type: oauth2
  upstream_identity: 'Sign in with Cloudflare, requesting one Cloudflare scope, "User Details: Read" (user id and email only).'
- applies_to: customer-deployed controlflare-cost-agent Worker (Cloudflare API)
  description: A Cloudflare scoped API token set by the customer as the CF_API_TOKEN secret on their own agent Worker. It never transits Controlflare. Controlflare holds only the agent URL and a pairing secret, and signs every request to the agent with that secret.
  name: cost-agent-cloudflare-token
  required_permissions:
  - Account · Workers Scripts · Edit
  - Zone · Workers Routes · Edit
  - Account · Account Analytics · Read
  - Zone · Zone · Read
  source: https://controlflare.com/#faq
  type: apiKey
slug: controlflare-com-authentication
source_filename: controlflare-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://controlflare.com/agents/\ndocs: https://controlflare.com/agents/#connect\nnote: No OpenAPI is published, so there is no derived securitySchemes baseline. These schemes are read from the docs. Auth endpoints were not called (probe-safety rule).\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  applies_to: https://app.controlflare.com/mcp\n  description: OAuth 2.1 for the remote MCP server. A first call to /mcp returns 401 with a WWW-Authenticate header naming the protected-resource metadata. The client then registers itself (dynamic client registration) and opens a consent page that names the client and lists what it can do. The user then signs in with Cloudflare.\n  upstream_identity: 'Sign in with Cloudflare, requesting one Cloudflare scope, \"User Details: Read\" (user id and email only).'\n  revocation: Remove the connection in the client. The next call gets a 401.\n  quote: A first call to /mcp comes back 401 with\
  \ a WWW-Authenticate header naming the protected-resource metadata; the client reads that, registers itself, and opens the consent page in your browser.\n- name: cost-agent-cloudflare-token\n  type: apiKey\n  applies_to: customer-deployed controlflare-cost-agent Worker (Cloudflare API)\n  description: A Cloudflare scoped API token set by the customer as the CF_API_TOKEN secret on their own agent Worker. It never transits Controlflare. Controlflare holds only the agent URL and a pairing secret, and signs every request to the agent with that secret.\n  required_permissions:\n  - Account · Workers Scripts · Edit\n  - Zone · Workers Routes · Edit\n  - Account · Account Analytics · Read\n  - Zone · Zone · Read\n  source: https://controlflare.com/#faq\n"
source_yaml_url: https://artifacts.apis.io/controlflare-com/authentication/controlflare-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cloudflare
- Cloudflare Workers
- Cost Management
- Budget Caps
- FinOps
- MCP
- Serverless
---
