---
api_key_in:
- header
api_specs:
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Indexes API
  slug: twelvelabs-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Tasks (Upload) API
  slug: twelvelabs-tasks-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Search API
  slug: twelvelabs-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Analyze / Generate API
  slug: twelvelabs-analyze-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Embed API
  slug: twelvelabs-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Twelvelabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: TwelveLabs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TwelveLabs
provider_slug: twelvelabs
scheme_count: 1
schemes:
- description: TwelveLabs API key sent in the `x-api-key` request header.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/twelvelabs-openapi.yml
  type: apiKey
slug: twelvelabs-authentication
source_filename: twelvelabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/twelvelabs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: TwelveLabs API key sent in the `x-api-key` request header.\n  sources:\n  - openapi/twelvelabs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/authentication/twelvelabs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Video Understanding
- Multimodal
- Search
- Embeddings
---
