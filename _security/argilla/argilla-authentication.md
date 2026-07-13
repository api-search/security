---
api_key_in:
- header
api_specs:
- filename: docs
  format: yaml
  label: Argilla REST API
  slug: argilla-rest-api
  spec_type: OpenAPI
  url: https://argilla.io/api/docs
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Argilla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argilla secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Argilla
provider_slug: argilla
scheme_count: 2
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Argilla-Api-Key
  sources:
  - openapi/argilla-rest-api-openapi.yml
  type: apiKey
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/argilla-rest-api-openapi.yml
  type: http
slug: argilla-authentication
source_filename: argilla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argilla-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Argilla-Api-Key\n  sources:\n  - openapi/argilla-rest-api-openapi.yml\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/argilla-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/authentication/argilla-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- data annotation
- LLM
- NLP
- RLHF
- machine learning
- datasets
- open source
- human feedback
- fine-tuning
- Hugging Face
---
