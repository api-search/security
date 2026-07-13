---
api_key_in:
- query
api_specs:
- filename: google-gemini-api-openapi.yml
  format: yaml
  label: Gemini API
  slug: gemini-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-gemini/refs/heads/main/openapi/google-gemini-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Google Gemini Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Gemini secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Google Gemini
provider_slug: google-gemini
scheme_count: 1
schemes:
- description: API key for authenticating requests. Obtain from Google AI Studio at https://aistudio.google.com/app/apikey.
  in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/google-gemini-api-openapi.yml
  type: apiKey
slug: google-gemini-authentication
source_filename: google-gemini-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-gemini-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key for authenticating requests. Obtain from Google AI Studio at https://aistudio.google.com/app/apikey.\n  sources:\n  - openapi/google-gemini-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-gemini/refs/heads/main/authentication/google-gemini-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agentic AI
- Artificial Intelligence
- Code Generation
- Embeddings
- Generative AI
- Image Generation
- LLM
- Machine Learning
- Multimodal
---
