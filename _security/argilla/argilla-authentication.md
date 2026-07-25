---
api_key_in:
- header
api_specs:
- filename: argilla-authentication-api-openapi.yml
  format: yaml
  label: Argilla Authentication API
  slug: argilla-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-authentication-api-openapi.yml
- filename: argilla-datasets-api-openapi.yml
  format: yaml
  label: Argilla datasets API
  slug: argilla-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-datasets-api-openapi.yml
- filename: argilla-fields-api-openapi.yml
  format: yaml
  label: Argilla fields API
  slug: argilla-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-fields-api-openapi.yml
- filename: argilla-info-api-openapi.yml
  format: yaml
  label: Argilla info API
  slug: argilla-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-info-api-openapi.yml
- filename: argilla-jobs-api-openapi.yml
  format: yaml
  label: Argilla jobs API
  slug: argilla-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-jobs-api-openapi.yml
- filename: argilla-metadata-properties-api-openapi.yml
  format: yaml
  label: Argilla metadata properties API
  slug: argilla-metadata-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-metadata-properties-api-openapi.yml
- filename: argilla-questions-api-openapi.yml
  format: yaml
  label: Argilla questions API
  slug: argilla-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-questions-api-openapi.yml
- filename: argilla-records-api-openapi.yml
  format: yaml
  label: Argilla records API
  slug: argilla-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-records-api-openapi.yml
- filename: argilla-responses-api-openapi.yml
  format: yaml
  label: Argilla responses API
  slug: argilla-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-responses-api-openapi.yml
- filename: argilla-settings-api-openapi.yml
  format: yaml
  label: Argilla settings API
  slug: argilla-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-settings-api-openapi.yml
- filename: argilla-suggestions-api-openapi.yml
  format: yaml
  label: Argilla suggestions API
  slug: argilla-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-suggestions-api-openapi.yml
- filename: argilla-users-api-openapi.yml
  format: yaml
  label: Argilla users API
  slug: argilla-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-users-api-openapi.yml
- filename: argilla-vectors-settings-api-openapi.yml
  format: yaml
  label: Argilla vectors-settings API
  slug: argilla-vectors-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-vectors-settings-api-openapi.yml
- filename: argilla-webhooks-api-openapi.yml
  format: yaml
  label: Argilla webhooks API
  slug: argilla-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-webhooks-api-openapi.yml
- filename: argilla-workspaces-api-openapi.yml
  format: yaml
  label: Argilla workspaces API
  slug: argilla-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argilla/refs/heads/main/openapi/argilla-workspaces-api-openapi.yml
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
