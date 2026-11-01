---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for OfoxAI
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Ofox Authentication
name_suffix: Authentication
oauth_flows: []
overview: NICE TALK declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: NICE TALK
provider_slug: ofox
scheme_count: 3
schemes:
- evidence: 'The OpenAI compatible protocol uses the Authorization header: Authorization: Bearer < your OFOXAI_API_KE Y >'
  header: Authorization
  how_to_obtain: Create a new API Key in the OfoxAI Console under Settings → API Keys.
  location: header
  name: Authorization
  type: apiKey
- evidence: 'The Anthropic native protocol uses the x-api-key header: x-api-key: < your OFOXAI_API_KE Y >'
  header: x-api-key
  how_to_obtain: Create a new API Key in the OfoxAI Console under Settings → API Keys.
  location: header
  name: x-api-key
  type: apiKey
- evidence: 'The Gemini native protocol uses the x-goog-api-key header or URL parameter: x-goog-api-key: < your OFOXAI_API_KE Y >'
  header: x-goog-api-key
  how_to_obtain: Create a new API Key in the OfoxAI Console under Settings → API Keys.
  location: header
  name: x-goog-api-key
  type: apiKey
slug: ofox-authentication
source_filename: ofox-authentication.yml
source_heading: Authentication Profile
source_url: https://ofox.ai/docs/develop/authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ofox.ai/docs/develop/authentication\nsources:\n- https://ofox.ai/docs/develop/authentication\n- https://ofox.ai/docs/develop/partner-oauth\n- https://ofox.ai/docs/develop\n- https://ofox.ai/quickstart\ndescription: Authentication methods for OfoxAI\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'The OpenAI compatible protocol uses the Authorization header: Authorization: Bearer < your OFOXAI_API_KE Y >'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a new API Key in the OfoxAI Console under Settings → API Keys.\n- type: apiKey\n  name: x-api-key\n  evidence: 'The Anthropic native protocol uses the x-api-key header: x-api-key: < your OFOXAI_API_KE Y >'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a new API Key in the OfoxAI Console under Settings → API Keys.\n- type: apiKey\n  name: x-goog-api-key\n  evidence: 'The\
  \ Gemini native protocol uses the x-goog-api-key header or URL parameter: x-goog-api-key: < your OFOXAI_API_KE Y >'\n  location: header\n  header: x-goog-api-key\n  how_to_obtain: Create a new API Key in the OfoxAI Console under Settings → API Keys.\nnote: OAuth integration details (token and authorize URLs, scopes, flows) are not provided on the referenced pages.\ndocs: https://ofox.ai/docs/develop/authentication\n"
source_yaml_url: https://artifacts.apis.io/ofox/authentication/ofox-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- LLM
- Platform
---
