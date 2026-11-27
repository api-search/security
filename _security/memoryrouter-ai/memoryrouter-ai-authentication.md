---
anonymous_access: false
api_key_in: []
api_specs:
- filename: memoryrouter-ai-openapi-generated.yml
  format: yaml
  label: MemoryRouter API
  slug: memoryrouter-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memoryrouter-ai/openapi/_ae-authored/memoryrouter-ai-openapi-generated.yml
auth_types: []
description: MemoryRouter authenticates requests using Memory Keys and optional Provider Keys.
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: MemoryRouter Authentication
name_suffix: Authentication
oauth_flows: []
overview: MemoryRouter declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: MemoryRouter
provider_slug: memoryrouter-ai
scheme_count: 5
schemes:
- evidence: 'Standard (Authorization header): curl -X POST https://api.memoryrouter.ai/v1/chat/completions \ -H "Authorization: Bearer mk_xxxxxxxxxxxxxxxx"'
  header: Authorization
  location: header
  name: Memory Key
  type: http-bearer
- evidence: 'Anthropic SDK style (x-api-key): curl -X POST https://api.memoryrouter.ai/v1/chat/completions \ -H "x-api-key: mk_xxxxxxxxxxxxxxxx"'
  header: x-api-key
  location: header
  name: Memory Key (x-api-key)
  type: apiKey
- evidence: 'Method A, Drop-in (recommended): provider key in Authorization , Memory Key in X-Memory-Key .'
  header: X-Memory-Key
  location: header
  name: Memory Key (X-Memory-Key)
  type: apiKey
- evidence: 'Method B, Explicit header: provider key in X-Provider-Key , Memory Key in Authorization .'
  header: Authorization
  location: header
  name: Provider Key (Authorization)
  type: http-bearer
- evidence: 'Method B, Explicit header: provider key in X-Provider-Key , Memory Key in Authorization .'
  header: X-Provider-Key
  location: header
  name: Provider Key (X-Provider-Key)
  type: apiKey
slug: memoryrouter-ai-authentication
source_filename: memoryrouter-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.memoryrouter.ai/authentication
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.memoryrouter.ai/authentication\nsources:\n- https://docs.memoryrouter.ai/authentication\n- https://docs.memoryrouter.ai/quickstart\n- https://docs.memoryrouter.ai/multi-agent\ndescription: MemoryRouter authenticates requests using Memory Keys and optional Provider Keys.\nschemes:\n- type: http-bearer\n  name: Memory Key\n  evidence: 'Standard (Authorization header): curl -X POST https://api.memoryrouter.ai/v1/chat/completions \\ -H \"Authorization: Bearer mk_xxxxxxxxxxxxxxxx\"'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: Memory Key (x-api-key)\n  evidence: 'Anthropic SDK style (x-api-key): curl -X POST https://api.memoryrouter.ai/v1/chat/completions \\ -H \"x-api-key: mk_xxxxxxxxxxxxxxxx\"'\n  location: header\n  header: x-api-key\n- type: apiKey\n  name: Memory Key (X-Memory-Key)\n  evidence: 'Method A, Drop-in (recommended): provider key\
  \ in Authorization , Memory Key in X-Memory-Key .'\n  location: header\n  header: X-Memory-Key\n- type: http-bearer\n  name: Provider Key (Authorization)\n  evidence: 'Method B, Explicit header: provider key in X-Provider-Key , Memory Key in Authorization .'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: Provider Key (X-Provider-Key)\n  evidence: 'Method B, Explicit header: provider key in X-Provider-Key , Memory Key in Authorization .'\n  location: header\n  header: X-Provider-Key\nnote: No OAuth2 flows are documented.\ndocs: https://docs.memoryrouter.ai/authentication\n"
source_yaml_url: https://artifacts.apis.io/memoryrouter-ai/authentication/memoryrouter-ai-authentication.yml
summary_line: 5 schemes
tags:
- Artificial Intelligence
- Memory
- Integration
- Platform
- Developers
---
