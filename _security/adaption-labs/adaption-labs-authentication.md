---
api_key_in: []
api_specs:
- filename: adaption-labs-datasets-api-openapi.yml
  format: yaml
  label: Adaption Labs Datasets API
  slug: adaption-labs-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaption-labs/refs/heads/main/openapi/adaption-labs-datasets-api-openapi.yml
- filename: adaption-labs-upload-api-openapi.yml
  format: yaml
  label: Adaption Labs Upload API
  slug: adaption-labs-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaption-labs/refs/heads/main/openapi/adaption-labs-upload-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Adaption Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adaption Labs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Adaption Labs
provider_slug: adaption-labs
scheme_count: 1
schemes:
- description: Static API key issued in the Adaption web app (Settings > API keys), sent as a Bearer token on every request.
  format: Bearer [example key]
  header: Authorization
  id: bearer
  in: header
  key_prefix: pt_live_
  scheme: bearer
  type: http
slug: adaption-labs-authentication
source_filename: adaption-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.adaptionlabs.ai/introduction/create-api-keys/index.md\ndocs: https://docs.adaptionlabs.ai/introduction/create-api-keys/index.md\napi: Adaptive Data API\nbase_url: https://api.prod.adaptionlabs.ai\nsummary: >-\n  Adaption authenticates programmatic access with a single API key presented as\n  an HTTP Bearer token. Keys are created in the web app under Settings > API keys,\n  shown once, and stored as a secret. The Python SDK reads the key from the\n  ADAPTION_API_KEY environment variable or an explicit api_key argument.\nschemes:\n- id: bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer [example key]'\n  key_prefix: pt_live_\n  description: >-\n    Static API key issued in the Adaption web app (Settings > API keys), sent as\n    a Bearer token on every request.\nenv:\n- name: ADAPTION_API_KEY\n  purpose: API key read by the Python SDK when no api_key argument is passed\n\
  - name: ADAPTION_BASE_URL\n  purpose: Overrides the default API base URL (https://api.prod.adaptionlabs.ai)\nkey_management:\n  create_url: https://adaptionlabs.ai/app/settings?tab=api_keys\n  rotation: Keys are shown once at creation and cannot be re-viewed; rotate by creating a new key.\n  third_party_credentials:\n  - provider: Kaggle\n    note: Kaggle API credentials must be registered under Settings > API keys before importing Kaggle datasets.\noauth2: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaption-labs/refs/heads/main/authentication/adaption-labs-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Machine Learning
- Training Data
- Datasets
- LLM
- Adaptive Data
- SDK
---
