---
anonymous_access: false
api_key_in: []
api_specs:
- filename: runbios-openapi-generated.yml
  format: yaml
  label: UltraSafe AI API
  slug: runbios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/runbios/openapi/_ae-authored/runbios-openapi-generated.yml
auth_types: []
description: Authentication schemes for Run BiOS API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Runbios Authentication
name_suffix: Authentication
oauth_flows: []
overview: UltraSafe AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: UltraSafe AI
provider_slug: runbios
scheme_count: 2
schemes:
- evidence: 'Surface Header Platform API — /api/* : datasets, training, deployments, billing. Also what the SDKs and MCP server call. X-API-Key: sk-bios-…'
  header: X-API-Key
  how_to_obtain: Create an API key in the Run BiOS console (Settings → API Keys) and use the value (starts with sk-bios-) as the X-API-Key header.
  location: header
  name: Platform API Key
  type: apiKey
- evidence: 'Serverless inference — /v1/* : chat completions, messages, models. OpenAI- and Anthropic-compatible. Authorization: Bearer bios-…'
  header: Authorization
  how_to_obtain: Use a serverless key (starts with bios-) as the Bearer token in the Authorization header.
  location: header
  name: Serverless Inference Bearer Token
  type: http-bearer
slug: runbios-authentication
source_filename: runbios-authentication.yml
source_heading: Authentication Profile
source_url: https://platform.runbios.ai/docs/api-overview
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://platform.runbios.ai/docs/api-overview\nsources:\n- https://platform.runbios.ai/docs/api-overview\n- https://platform.runbios.ai/docs/api-keys\ndescription: Authentication schemes for Run BiOS API\nschemes:\n- type: apiKey\n  name: Platform API Key\n  evidence: 'Surface Header Platform API — /api/* : datasets, training, deployments, billing. Also what the SDKs and MCP server call. X-API-Key:\n    sk-bios-…'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key in the Run BiOS console (Settings → API Keys) and use the value (starts with sk-bios-) as the X-API-Key header.\n- type: http-bearer\n  name: Serverless Inference Bearer Token\n  evidence: 'Serverless inference — /v1/* : chat completions, messages, models. OpenAI- and Anthropic-compatible. Authorization: Bearer bios-…'\n  location: header\n  header: Authorization\n  how_to_obtain: Use a serverless\
  \ key (starts with bios-) as the Bearer token in the Authorization header.\ndocs: https://platform.runbios.ai/docs/api-overview\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/runbios/authentication/runbios-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Enterprise
- Platform
- Training
- Inference
---
