---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for khive API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: khive AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: khive AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: khive AI
provider_slug: khive-ai
scheme_count: 1
schemes:
- evidence: Cursor connects to khive over HTTP with an API key. Its MCP configuration file names an environment variable, and Cursor reads the key from it.
  header: Authorization
  how_to_obtain: Create an API key in the khive dashboard (https://khive.ai/dashboard/keys) and set it in an environment variable (e.g., KHIVE_API_KEY).
  location: header
  name: API Key
  type: apiKey
slug: khive-ai-authentication
source_filename: khive-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.khive.ai/docs/connect/cursor
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.khive.ai/docs/connect/cursor\nsources:\n- https://www.khive.ai/docs/connect/cursor\n- https://www.khive.ai/docs/account\n- https://www.khive.ai/docs/connect/claude-code\n- https://www.khive.ai/docs/connect/codex\ndescription: Authentication schemes for khive API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Cursor connects to khive over HTTP with an API key. Its MCP configuration file names an environment variable, and Cursor reads the\n    key from it.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the khive dashboard (https://khive.ai/dashboard/keys) and set it in an environment variable (e.g., KHIVE_API_KEY).\nnote: OAuth flows are mentioned for sign‑in, but the documentation does not provide token or authorize URLs, scopes, or flow details, so no OAuth\n  scheme is recorded.\ndocs: https://www.khive.ai/docs/connect/cursor\n"
source_yaml_url: https://artifacts.apis.io/khive-ai/authentication/khive-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Cognitive Infrastructure
- Memory
- Knowledge Graph
- Multi-Agent
---
