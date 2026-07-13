---
api_key_in:
- header
api_specs:
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Items & Upload API
  slug: items-upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Annotations API
  slug: annotations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Workflows & Stages API
  slug: workflows-stages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Annotation Classes API
  slug: classes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Exports API
  slug: exports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: V7 Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: V7 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: V7
provider_slug: v7-labs
scheme_count: 1
schemes:
- description: 'Team-scoped API key sent as `Authorization: ApiKey {key}`. Generate keys at https://darwin.v7labs.com/?settings=api-keys. Key permissions determine which operations are allowed.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/v7-labs-openapi.yml
  type: apiKey
slug: v7-labs-authentication
source_filename: v7-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/v7-labs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Team-scoped API key sent as `Authorization: ApiKey {key}`. Generate keys at\n    https://darwin.v7labs.com/?settings=api-keys. Key permissions determine which operations\n    are allowed.'\n  sources:\n  - openapi/v7-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/authentication/v7-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Training Data
- Data Labeling
- Annotation
- Document AI
- Computer Vision
---
