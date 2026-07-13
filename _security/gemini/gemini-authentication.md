---
api_key_in:
- header
- query
api_specs:
- filename: rest
  format: yaml
  label: Gemini REST API
  slug: gemini-rest-api
  spec_type: OpenAPI
  url: https://generativelanguage.googleapis.com/$discovery/rest?version=v1beta&key=YOUR_API_KEY
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gemini Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gemini secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gemini
provider_slug: gemini
scheme_count: 2
schemes:
- description: Gemini API key from Google AI Studio
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/gemini-openapi.yml
  type: apiKey
- description: Gemini API key passed via header
  in: header
  name: apiKeyHeader
  parameter: x-goog-api-key
  sources:
  - openapi/gemini-openapi.yml
  type: apiKey
slug: gemini-authentication
source_filename: gemini-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gemini-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Gemini API key from Google AI Studio\n  sources:\n  - openapi/gemini-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-goog-api-key\n  description: Gemini API key passed via header\n  sources:\n  - openapi/gemini-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemini/refs/heads/main/authentication/gemini-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Agents
- Artificial Intelligence
- Audio Understanding
- Batch Processing
- Deep Research
- Document Understanding
- Embeddings
- Function Calling
- Generative Ai
- Image Generation
- Large Language Models
- Machine Learning
- Multimodal
- Structured Output
- Text-To-Speech
- Video Generation
- Video Understanding
---
