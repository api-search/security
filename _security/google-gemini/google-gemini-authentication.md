---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-gemini-auth-tokens-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Auth Tokens API
  slug: google-gemini-auth-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-auth-tokens-api-openapi.yml
- filename: google-gemini-batches-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Batches API
  slug: google-gemini-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-batches-api-openapi.yml
- filename: google-gemini-corpora-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Corpora API
  slug: google-gemini-corpora-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-corpora-api-openapi.yml
- filename: google-gemini-dynamic-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Dynamic API
  slug: google-gemini-dynamic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-dynamic-api-openapi.yml
- filename: google-gemini-environments-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Environments API
  slug: google-gemini-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-environments-api-openapi.yml
- filename: google-gemini-files-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Files API
  slug: google-gemini-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-files-api-openapi.yml
- filename: google-gemini-media-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Media API
  slug: google-gemini-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-media-api-openapi.yml
- filename: google-gemini-models-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Models API
  slug: google-gemini-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-models-api-openapi.yml
- filename: google-gemini-cachedcontents-api-openapi.yml
  format: yaml
  label: Google Gemini Cached Contents API
  slug: google-gemini-cachedcontents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-cachedcontents-api-openapi.yml
- filename: google-gemini-filesearchstores-api-openapi.yml
  format: yaml
  label: Google Gemini File Search Stores API
  slug: google-gemini-filesearchstores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-filesearchstores-api-openapi.yml
- filename: google-gemini-generatedfiles-api-openapi.yml
  format: yaml
  label: Google Gemini Generated Files API
  slug: google-gemini-generatedfiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-generatedfiles-api-openapi.yml
- filename: google-gemini-tunedmodels-api-openapi.yml
  format: yaml
  label: Google Gemini Tuned Models API
  slug: google-gemini-tunedmodels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-tunedmodels-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/google-gemini/authentication/google-gemini-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Agents
- Artificial Intelligence
- Code Generation
- Embeddings
- Generative AI
- Image Generation
- LLM
- Machine Learning
- Multi-Modal
- Real-Time
- Foundation Models
- Agents
- Audio Understanding
- Batch Processing
- Deep Research
- Document Understanding
- Function Calling
- Structured Output
- Text-to-Speech
- Video Generation
- Video Understanding
---
