---
api_key_in:
- header
api_specs:
- filename: llmwhisperer-extraction-api-openapi.yml
  format: yaml
  label: LLMWhisperer Extraction API
  slug: llmwhisperer-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-extraction-api-openapi.yml
- filename: llmwhisperer-highlights-api-openapi.yml
  format: yaml
  label: LLMWhisperer Highlights API
  slug: llmwhisperer-highlights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-highlights-api-openapi.yml
- filename: llmwhisperer-retrieve-api-openapi.yml
  format: yaml
  label: LLMWhisperer Retrieve API
  slug: llmwhisperer-retrieve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-retrieve-api-openapi.yml
- filename: llmwhisperer-status-api-openapi.yml
  format: yaml
  label: LLMWhisperer Status API
  slug: llmwhisperer-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-status-api-openapi.yml
- filename: llmwhisperer-webhooks-api-openapi.yml
  format: yaml
  label: LLMWhisperer Webhooks API
  slug: llmwhisperer-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Llmwhisperer Authentication
name_suffix: Authentication
oauth_flows: []
overview: LLMWhisperer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LLMWhisperer
provider_slug: llmwhisperer
scheme_count: 1
schemes:
- description: LLMWhisperer API key passed in the unstract-key request header.
  in: header
  name: unstractKey
  parameter: unstract-key
  sources:
  - openapi/llmwhisperer-openapi.yml
  type: apiKey
slug: llmwhisperer-authentication
source_filename: llmwhisperer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/llmwhisperer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: unstractKey\n  type: apiKey\n  in: header\n  parameter: unstract-key\n  description: LLMWhisperer API key passed in the unstract-key request header.\n  sources:\n  - openapi/llmwhisperer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/authentication/llmwhisperer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- LLM
- Document Extraction
- OCR
- Text Extraction
---
