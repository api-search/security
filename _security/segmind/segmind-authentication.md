---
api_key_in:
- header
api_specs:
- filename: segmind-account-api-openapi.yml
  format: yaml
  label: Segmind Account API
  slug: segmind-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-account-api-openapi.yml
- filename: segmind-fine-tuning-api-openapi.yml
  format: yaml
  label: Segmind Fine-tuning API
  slug: segmind-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-fine-tuning-api-openapi.yml
- filename: segmind-inference-api-openapi.yml
  format: yaml
  label: Segmind Inference API
  slug: segmind-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-inference-api-openapi.yml
- filename: segmind-storage-api-openapi.yml
  format: yaml
  label: Segmind Storage API
  slug: segmind-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-storage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Segmind Authentication
name_suffix: Authentication
oauth_flows: []
overview: Segmind secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Segmind
provider_slug: segmind
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/segmind-openapi.yml
  type: apiKey
slug: segmind-authentication
source_filename: segmind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/segmind-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/segmind-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/authentication/segmind-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
