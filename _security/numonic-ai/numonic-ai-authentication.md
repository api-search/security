---
anonymous_access: false
api_key_in: []
api_specs:
- filename: numonic-ai-openapi-generated.yml
  format: yaml
  label: Numonic Ltd. API
  slug: numonic-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numonic-ai/openapi/_ae-authored/numonic-ai-openapi-generated.yml
auth_types: []
description: 'Numonic supports two authentication methods: OAuth 2.0 (dynamic discovery) and API‑key.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Numonic Ltd. Authentication
name_suffix: Authentication
oauth_flows: []
overview: Numonic Ltd. declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Numonic Ltd.
provider_slug: numonic-ai
scheme_count: 2
schemes:
- evidence: You don't configure anything extra. The client calls the endpoint, is told where Numonic's authorization details live ( /.well-known/oauth-protected-resource/mcp ), and registers itself.
  name: OAuth 2.0
  type: oauth2
- evidence: 'Send the key in a header only ( Authorization: Bearer napi_… or X-API-Key: napi_… ); a key in the URL is rejected.'
  header: Authorization or X-API-Key
  how_to_obtain: Create a key in Settings → Workspace → Connected Agents; the key starts with napi_ and is shown once.
  location: header
  name: API key
  type: apiKey
slug: numonic-ai-authentication
source_filename: numonic-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.numonic.ai/docs/api/mcp/quickstart?client=perplexity
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.numonic.ai/docs/api/mcp/quickstart?client=perplexity\nsources:\n- https://www.numonic.ai/docs/api/mcp/quickstart?client=perplexity\n- https://www.numonic.ai/docs/api/mcp/quickstart?client=perplexity&auth=api-key\n- https://www.numonic.ai/docs/api/mcp/quickstart?client=copilot-studio\ndescription: 'Numonic supports two authentication methods: OAuth 2.0 (dynamic discovery) and API‑key.'\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: You don't configure anything extra. The client calls the endpoint, is told where Numonic's authorization details live ( /.well-known/oauth-protected-resource/mcp\n    ), and registers itself.\n- type: apiKey\n  name: API key\n  evidence: 'Send the key in a header only ( Authorization: Bearer napi_… or X-API-Key: napi_… ); a key in the URL is rejected.'\n  location: header\n  header: Authorization or X-API-Key\n  how_to_obtain: Create\
  \ a key in Settings → Workspace → Connected Agents; the key starts with napi_ and is shown once.\ndocs: https://www.numonic.ai/docs/api/mcp/quickstart?client=perplexity\n"
source_yaml_url: https://artifacts.apis.io/numonic-ai/authentication/numonic-ai-authentication.yml
summary_line: 2 schemes
tags:
- Asset Management
- AI Generation
- Creative Studios
- Compliance
- Workflow Capture
- Midjourney
- ComfyUI
---
