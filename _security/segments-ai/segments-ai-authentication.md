---
api_key_in:
- header
api_specs:
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Samples API
  slug: samples
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Labels API
  slug: labels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Labelsets API
  slug: labelsets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Releases API
  slug: releases
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Segments Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Segments.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Segments.ai
provider_slug: segments-ai
scheme_count: 1
schemes:
- description: Send your API key in the Authorization header using the value `APIKey YOUR_API_KEY`. Keys are generated in the Segments.ai account settings.
  in: header
  name: APIKey
  parameter: Authorization
  sources:
  - openapi/segments-ai-openapi.yml
  type: apiKey
slug: segments-ai-authentication
source_filename: segments-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/segments-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Send your API key in the Authorization header using the value `APIKey YOUR_API_KEY`.\n    Keys are generated in the Segments.ai account settings.\n  sources:\n  - openapi/segments-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/authentication/segments-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Labeling
- Computer Vision
- Point Cloud
- Annotation
- Machine Learning
---
