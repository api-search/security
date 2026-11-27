---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getlinkintel-com-api-openapi.json
  format: json
  label: LinkIntel API API
  slug: linkintel-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlinkintel-com/openapi/_original/getlinkintel-com-api-openapi.json
auth_types: []
description: Authentication methods for LinkIntel MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LinkIntel Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkIntel declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LinkIntel
provider_slug: getlinkintel-com
scheme_count: 2
schemes:
- evidence: OAuth 2.1 handles authentication in your browser with no token to type or share.
  name: OAuth 2.1
  type: oauth2
- evidence: If your client does not support OAuth 2.1, get a bearer token instead. Go to https://www.getlinkintel.com/agent , create an account with Google, review and confirm the $39/month offer, then copy the private MCP handoff shown on /setup.
  header: Authorization
  how_to_obtain: Create an account at https://www.getlinkintel.com/agent and copy the private MCP handoff token (starts with lnki_) shown on /setup.
  location: header
  name: Private bearer token fallback
  type: http-bearer
slug: getlinkintel-com-authentication
source_filename: getlinkintel-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.getlinkintel.com/SKILL.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.getlinkintel.com/SKILL.md\nsources:\n- https://www.getlinkintel.com/SKILL.md\n- https://www.getlinkintel.com/connect\n- https://www.getlinkintel.com/docs/mcp\ndescription: Authentication methods for LinkIntel MCP server\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: OAuth 2.1 handles authentication in your browser with no token to type or share.\n- type: http-bearer\n  name: Private bearer token fallback\n  evidence: If your client does not support OAuth 2.1, get a bearer token instead. Go to https://www.getlinkintel.com/agent , create an account\n    with Google, review and confirm the $39/month offer, then copy the private MCP handoff shown on /setup.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account at https://www.getlinkintel.com/agent and copy the private MCP handoff token (starts with lnki_) shown on /setup.\ndocs: https://www.getlinkintel.com/SKILL.md\n"
source_yaml_url: https://artifacts.apis.io/getlinkintel-com/authentication/getlinkintel-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- MCP
- Content
- Analytics
---
