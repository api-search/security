---
anonymous_access: false
api_key_in: []
api_specs:
- filename: stealthgpt-ai-stealthify-api-openapi.yml
  format: yaml
  label: StealthGPT Stealthify API
  slug: stealthgpt-ai-stealthify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stealthgpt-ai/openapi/stealthgpt-ai-stealthify-api-openapi.yml
auth_types: []
description: StealthGPT uses a simple API token passed in a custom header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: StealthGPT Authentication
name_suffix: Authentication
oauth_flows: []
overview: StealthGPT declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: StealthGPT
provider_slug: stealthgpt-ai
scheme_count: 1
schemes:
- evidence: Include your API token in the headers of all requests to the StealthGPT API.
  header: api-token
  how_to_obtain: Find your API token in the StealthGPT Dashboard under the "API Key" tab.
  location: header
  name: api-token
  type: apiKey
slug: stealthgpt-ai-authentication
source_filename: stealthgpt-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.stealthgpt.ai/api-reference/authentication.md
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.stealthgpt.ai/api-reference/authentication.md\nsources:\n- https://docs.stealthgpt.ai/api-reference/authentication.md\n- https://docs.stealthgpt.ai/api-reference/quickstart.md\ndescription: StealthGPT uses a simple API token passed in a custom header.\nschemes:\n- type: apiKey\n  name: api-token\n  evidence: Include your API token in the headers of all requests to the StealthGPT API.\n  location: header\n  header: api-token\n  how_to_obtain: Find your API token in the StealthGPT Dashboard under the \"API Key\" tab.\nnote: No OAuth2, HTTP Basic, Bearer, JWT, HMAC, mTLS, or other authentication schemes are documented.\ndocs: https://docs.stealthgpt.ai/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/stealthgpt-ai/authentication/stealthgpt-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Text-Humanization
- Detection
---
