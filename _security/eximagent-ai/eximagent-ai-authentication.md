---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eximagent-ai-openapi-generated.yml
  format: yaml
  label: EximAgent API
  slug: eximagent-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eximagent-ai/openapi/_ae-authored/eximagent-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for EximAgent
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: EximAgent Authentication
name_suffix: Authentication
oauth_flows: []
overview: EximAgent declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: EximAgent
provider_slug: eximagent-ai
scheme_count: 2
schemes:
- evidence: 'Send the key in the Authorization header. For example, with the key already stored in the EXIMAGENT_API_KEY environment variable:'
  header: Authorization
  how_to_obtain: Create a key in Settings → API keys in the product app and save the secret.
  location: header
  name: API key
  type: apiKey
- evidence: Authentication OAuth 2.1 with dynamic client registration and PKCE; Google sign-in
  how_to_obtain: Use the hosted MCP server which performs OAuth sign‑in; the same endpoint is used for all users.
  name: OAuth 2.1 (dynamic client registration, PKCE)
  type: oauth2
slug: eximagent-ai-authentication
source_filename: eximagent-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://eximagent.ai/docs/integrations/api-keys
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://eximagent.ai/docs/integrations/api-keys\nsources:\n- https://eximagent.ai/docs/integrations/api-keys\n- https://eximagent.ai/docs/get-started/authenticate\n- https://eximagent.ai/docs/integrations/mcp\n- https://eximagent.ai/docs/agents\ndescription: Authentication methods for EximAgent\nschemes:\n- type: apiKey\n  name: API key\n  evidence: 'Send the key in the Authorization header. For example, with the key already stored in the EXIMAGENT_API_KEY environment variable:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings → API keys in the product app and save the secret.\n- type: oauth2\n  name: OAuth 2.1 (dynamic client registration, PKCE)\n  evidence: Authentication OAuth 2.1 with dynamic client registration and PKCE; Google sign-in\n  how_to_obtain: Use the hosted MCP server which performs OAuth sign‑in; the same endpoint is used for\
  \ all users.\ndocs: https://eximagent.ai/docs/integrations/api-keys\n"
source_yaml_url: https://artifacts.apis.io/eximagent-ai/authentication/eximagent-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Trade
- Export
- Market Research
- Software-as-a-Service
---
