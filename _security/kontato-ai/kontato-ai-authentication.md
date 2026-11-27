---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kontato-ai-openapi-generated.yml
  format: yaml
  label: Kontato API
  slug: kontato-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kontato-ai/openapi/_ae-authored/kontato-ai-openapi-generated.yml
auth_types: []
description: Authentication uses an API key provided as a Bearer token in the Authorization header. The API key is returned once during account signup and must be stored securely. All endpoints except the signup call require the header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kontato Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kontato declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kontato
provider_slug: kontato-ai
scheme_count: 1
schemes:
- evidence: 'Transporte: sempre Authorization: Bearer <api_key> em HTTPS, em todos os endpoints exceto o signup.'
  header: Authorization
  how_to_obtain: Create an account via POST /v1/signup; the response includes the api_key.
  location: header
  name: api_key
  type: apiKey
slug: kontato-ai-authentication
source_filename: kontato-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://kontato.ai/docs/agent/authentication.md
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kontato.ai/docs/agent/authentication.md\nsources:\n- https://kontato.ai/docs/agent/authentication.md\n- https://kontato.ai/docs/agent/quickstart.md\n- https://kontato.ai/docs/agent/mcp-setup.md\ndescription: Authentication uses an API key provided as a Bearer token in the Authorization header. The API key is returned once during account\n  signup and must be stored securely. All endpoints except the signup call require the header.\nschemes:\n- type: apiKey\n  name: api_key\n  evidence: 'Transporte: sempre Authorization: Bearer <api_key> em HTTPS, em todos os endpoints exceto o signup.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account via POST /v1/signup; the response includes the api_key.\nnote: OAuth login is mentioned for the MCP endpoint but no token or authorize URLs, flow types, or scopes are provided on the pages, so no OAuth\n  scheme\
  \ is recorded.\ndocs: https://kontato.ai/docs/agent/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/kontato-ai/authentication/kontato-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Communications
- WhatsApp
- Automation
---
