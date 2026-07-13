---
api_key_in:
- header
api_specs:
- filename: voxel51-openapi.yml
  format: yaml
  label: FiftyOne SDK (Python)
  slug: fiftyone-sdk-python
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxel51/refs/heads/main/openapi/voxel51-openapi.yml
- filename: voxel51-openapi.yml
  format: yaml
  label: FiftyOne Enterprise Management SDK / API
  slug: fiftyone-enterprise-management-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxel51/refs/heads/main/openapi/voxel51-openapi.yml
- filename: voxel51-openapi.yml
  format: yaml
  label: FiftyOne Plugins & Operators
  slug: fiftyone-plugins-operators
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxel51/refs/heads/main/openapi/voxel51-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Voxel51 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voxel51 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Voxel51
provider_slug: voxel51
scheme_count: 1
schemes:
- description: FiftyOne Enterprise API key. Used by the SDK over the authenticated API connection (FIFTYONE_API_KEY). Keys are per-user and enforce that user's roles and dataset permissions.
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/voxel51-openapi.yml
  type: apiKey
slug: voxel51-authentication
source_filename: voxel51-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/voxel51-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: FiftyOne Enterprise API key. Used by the SDK over the authenticated API connection\n    (FIFTYONE_API_KEY). Keys are per-user and enforce that user's roles and dataset permissions.\n  sources:\n  - openapi/voxel51-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voxel51/refs/heads/main/authentication/voxel51-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Computer Vision
- Datasets
- Machine Learning
- Python SDK
---
