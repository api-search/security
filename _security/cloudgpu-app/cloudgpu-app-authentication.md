---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudgpu-app-api-openapi.json
  format: json
  label: CloudGPU API API
  slug: cloudgpu-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudgpu-app/openapi/_original/cloudgpu-app-api-openapi.json
auth_types: []
description: Authentication for CloudGPU API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CloudGPU Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudGPU declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CloudGPU
provider_slug: cloudgpu-app
scheme_count: 1
schemes:
- evidence: 'You can rule out the tool entirely with one cURL call: curl https://cloudgpu.app/v1/chat/completions \ -H "Content-Type: application/json" \ -H "Authorization: Bearer cgw-sk-..." \ -d ''{"model": "claude-sonnet-5-5","messages": [{"role": "user", "content": "ok?"}]}'''
  header: Authorization
  how_to_obtain: Create a key in the API console; it starts with cgw-sk-.
  location: header
  name: Bearer token
  type: http-bearer
slug: cloudgpu-app-authentication
source_filename: cloudgpu-app-authentication.yml
source_heading: Authentication Profile
source_url: https://cloudgpu.app/blog/self-host-llm-vs-api-break-even-2026
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cloudgpu.app/blog/self-host-llm-vs-api-break-even-2026\nsources:\n- https://cloudgpu.app/blog/self-host-llm-vs-api-break-even-2026\n- https://cloudgpu.app/blog/claude-in-cursor-cline-continue-setup-2026\ndescription: Authentication for CloudGPU API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'You can rule out the tool entirely with one cURL call: curl https://cloudgpu.app/v1/chat/completions \\ -H \"Content-Type: application/json\"\n    \\ -H \"Authorization: Bearer cgw-sk-...\" \\ -d ''{\"model\": \"claude-sonnet-5-5\",\"messages\": [{\"role\": \"user\", \"content\": \"ok?\"}]}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the API console; it starts with cgw-sk-.\nnote: No other authentication schemes (apiKey, oauth2, etc.) are documented on the provided pages.\ndocs: https://cloudgpu.app/blog/self-host-llm-vs-api-break-even-2026\n"
source_yaml_url: https://artifacts.apis.io/cloudgpu-app/authentication/cloudgpu-app-authentication.yml
summary_line: 1 scheme
tags:
- Cloud GPU
- GPU Rental
- AI Models
- OpenAI-Compatible
- Developer Platform
- Billing
---
