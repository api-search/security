---
anonymous_access: false
api_key_in: []
api_specs:
- filename: airouter-ai-router-api-api-openapi.yml
  format: yaml
  label: AI Router AI Router API
  slug: airouter-ai-router-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airouter/refs/heads/main/openapi/airouter-ai-router-api-api-openapi.yml
- filename: airouter-chat-completions-api-openapi.yml
  format: yaml
  label: AI Router Chat Completions API
  slug: airouter-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airouter/refs/heads/main/openapi/airouter-chat-completions-api-openapi.yml
auth_types: []
description: API key authentication using a bearer token
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Airouter Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Router declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AI Router
provider_slug: airouter
scheme_count: 1
schemes:
- evidence: 'Use the key as a bearer token ( Authorization: Bearer <API-KEY> ) for every request.'
  header: Authorization
  how_to_obtain: Create a key in the dashboard under Settings → API Keys.
  location: header
  name: API Key
  type: http-bearer
slug: airouter-authentication
source_filename: airouter-authentication.yml
source_heading: Authentication Profile
source_url: https://airouter.io/docs/quickstart/getting-started
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://airouter.io/docs/quickstart/getting-started\nsources:\n- https://airouter.io/docs/quickstart/getting-started\n- https://airouter.io/docs/quickstart/provider-keys\n- https://airouter.io/docs/quickstart/using-python-sdk\ndescription: API key authentication using a bearer token\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Use the key as a bearer token ( Authorization: Bearer <API-KEY> ) for every request.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard under Settings → API Keys.\ndocs: https://airouter.io/docs/quickstart/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airouter/refs/heads/main/authentication/airouter-authentication.yml
summary_line: 1 scheme
tags:
- LLM Cost Optimization
- Model Routing
- Enterprise AI
- Privacy
---
