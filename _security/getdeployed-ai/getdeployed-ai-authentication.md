---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes described on the Deployed AI MCP Governance page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Deployed AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deployed AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Deployed AI
provider_slug: getdeployed-ai
scheme_count: 2
schemes:
- evidence: It is built on OAuth 2.1 , the same family of standards behind “Sign in with Microsoft” or “Sign in with Google”.
  how_to_obtain: User signs in to the system and approves access; the AI client receives a token, not the password.
  name: OAuth 2.1
  type: oauth2
- evidence: Local servers that run on a person’s own machine over stdio do not use it; they take credentials from their environment, which in practice often means an API key in a configuration file.
  how_to_obtain: Use a shared key stored in a configuration file.
  location: configuration file
  name: Service account API key
  type: apiKey
slug: getdeployed-ai-authentication
source_filename: getdeployed-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://getdeployed.ai/blog/mcp-governance
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getdeployed.ai/blog/mcp-governance\nsources:\n- https://getdeployed.ai/blog/mcp-governance\ndescription: Authentication schemes described on the Deployed AI MCP Governance page.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: It is built on OAuth 2.1 , the same family of standards behind “Sign in with Microsoft” or “Sign in with Google”.\n  how_to_obtain: User signs in to the system and approves access; the AI client receives a token, not the password.\n- type: apiKey\n  name: Service account API key\n  evidence: Local servers that run on a person’s own machine over stdio do not use it; they take credentials from their environment, which in\n    practice often means an API key in a configuration file.\n  location: configuration file\n  how_to_obtain: Use a shared key stored in a configuration file.\ndocs: https://getdeployed.ai/blog/mcp-governance\n"
source_yaml_url: https://artifacts.apis.io/getdeployed-ai/authentication/getdeployed-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- MCP
- Governance
- Enterprise
---
