---
api_key_in:
- query
api_specs:
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Datasets API
  slug: lightly-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Samples and Embeddings API
  slug: lightly-samples-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Datasources API
  slug: lightly-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Selection and Active Learning API
  slug: lightly-selection-active-learning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Jobs and Tags API
  slug: lightly-jobs-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lightly Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightly secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lightly
provider_slug: lightly-ai
scheme_count: 2
schemes:
- description: LightlyOne API token passed as the `token` query parameter. Find your token in the preferences menu of the LightlyOne Platform.
  in: query
  name: ApiKeyAuth
  parameter: token
  sources:
  - openapi/lightly-ai-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'Public JWT bearer token passed in the `Authorization: Bearer <token>` header for browser / public-token authenticated calls.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lightly-ai-openapi.yml
  type: http
slug: lightly-ai-authentication
source_filename: lightly-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lightly-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: LightlyOne API token passed as the `token` query parameter. Find your token in\n    the preferences menu of the LightlyOne Platform.\n  sources:\n  - openapi/lightly-ai-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Public JWT bearer token passed in the `Authorization: Bearer <token>` header\n    for browser / public-token authenticated calls.'\n  sources:\n  - openapi/lightly-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/authentication/lightly-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Computer Vision
- Data Curation
- Active Learning
- Embeddings
---
