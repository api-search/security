---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kitforai-batch-api-openapi.yml
  format: yaml
  label: Kit For AI Batch API
  slug: kitforai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/openapi/kitforai-batch-api-openapi.yml
- filename: kitforai-convert-api-openapi.yml
  format: yaml
  label: Kit For AI Convert API
  slug: kitforai-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/openapi/kitforai-convert-api-openapi.yml
- filename: kitforai-knowledge-bases-api-openapi.yml
  format: yaml
  label: Kit For AI Knowledge Bases API
  slug: kitforai-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/openapi/kitforai-knowledge-bases-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kitforai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kit For AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kit For AI
provider_slug: kitforai
scheme_count: 1
schemes:
- evidence: Every request authenticates with an API key. Create one in Settings → API keys and send it in the x‑api‑key header.
  header: x-api-key
  how_to_obtain: Create an API key in Settings → API keys.
  location: header
  name: API Key
  type: apiKey
slug: kitforai-authentication
source_filename: kitforai-authentication.yml
source_heading: Authentication Profile
source_url: https://kitforai.com/docs
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kitforai.com/docs\nsources:\n- https://kitforai.com/docs\n- https://kitforai.com/blog/reduce-llm-token-costs\n- https://kitforai.com/llm-setup\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every request authenticates with an API key. Create one in Settings → API keys and send it in the x‑api‑key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create an API key in Settings → API keys.\ndocs: https://kitforai.com/docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/authentication/kitforai-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Memory
- DocumentConversion
- RetrievalAugmentedGeneration
- KnowledgeBase
---
