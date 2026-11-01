---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for reviewpaper.ai
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Reviewpaper Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: reviewpaper-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: reviewpaper-ai
provider_slug: reviewpaper-ai
scheme_count: 2
schemes:
- evidence: Signed-in MCP endpoint (OAuth) https://reviewpaper.ai/mcp/account
  name: OAuth
  type: oauth2
- evidence: No account, no key.
  name: none
  type: other
slug: reviewpaper-ai-authentication
source_filename: reviewpaper-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://reviewpaper.ai/developers
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://reviewpaper.ai/developers\nsources:\n- https://reviewpaper.ai/developers\ndescription: Authentication schemes for reviewpaper.ai\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Signed-in MCP endpoint (OAuth) https://reviewpaper.ai/mcp/account\n- type: other\n  name: none\n  evidence: No account, no key.\ndocs: https://reviewpaper.ai/developers\n"
source_yaml_url: https://artifacts.apis.io/reviewpaper-ai/authentication/reviewpaper-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Peer Review
- Academic
- NLP
- Research Tools
---
