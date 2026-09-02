---
api_key_in:
- header
api_specs:
- filename: pika-labs-cancel-api-openapi.yml
  format: yaml
  label: Pika Labs Cancel API
  slug: pika-labs-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pika-labs/refs/heads/main/openapi/pika-labs-cancel-api-openapi.yml
- filename: pika-labs-result-api-openapi.yml
  format: yaml
  label: Pika Labs Result API
  slug: pika-labs-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pika-labs/refs/heads/main/openapi/pika-labs-result-api-openapi.yml
- filename: pika-labs-status-api-openapi.yml
  format: yaml
  label: Pika Labs Status API
  slug: pika-labs-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pika-labs/refs/heads/main/openapi/pika-labs-status-api-openapi.yml
- filename: pika-labs-submission-api-openapi.yml
  format: yaml
  label: Pika Labs Submission API
  slug: pika-labs-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pika-labs/refs/heads/main/openapi/pika-labs-submission-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pika Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pika Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pika Labs
provider_slug: pika-labs
scheme_count: 1
schemes:
- description: 'fal.ai API key sent as `Authorization: Key $FAL_KEY`.'
  in: header
  name: falKey
  parameter: Authorization
  sources:
  - openapi/pika-labs-openapi.yml
  type: apiKey
slug: pika-labs-authentication
source_filename: pika-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pika-labs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: falKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'fal.ai API key sent as `Authorization: Key $FAL_KEY`.'\n  sources:\n  - openapi/pika-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pika-labs/refs/heads/main/authentication/pika-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Video Generation
- Text-to-Video
- Multi-Modal
- Generative
---
