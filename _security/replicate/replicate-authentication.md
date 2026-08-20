---
api_key_in: []
api_specs:
- filename: replicate-accounts-api-openapi.yml
  format: yaml
  label: Replicate Accounts API
  slug: replicate-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-accounts-api-openapi.yml
- filename: replicate-cancel-api-openapi.yml
  format: yaml
  label: Replicate Cancel API
  slug: replicate-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-cancel-api-openapi.yml
- filename: replicate-collections-api-openapi.yml
  format: yaml
  label: Replicate Collections API
  slug: replicate-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-collections-api-openapi.yml
- filename: replicate-deployments-api-openapi.yml
  format: yaml
  label: Replicate Deployments API
  slug: replicate-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-deployments-api-openapi.yml
- filename: replicate-hardware-api-openapi.yml
  format: yaml
  label: Replicate Hardware API
  slug: replicate-hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-hardware-api-openapi.yml
- filename: replicate-model-api-openapi.yml
  format: yaml
  label: Replicate Model API
  slug: replicate-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-model-api-openapi.yml
- filename: replicate-models-api-openapi.yml
  format: yaml
  label: Replicate Models API
  slug: replicate-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-models-api-openapi.yml
- filename: replicate-name-api-openapi.yml
  format: yaml
  label: Replicate Name API
  slug: replicate-name-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-name-api-openapi.yml
- filename: replicate-owner-api-openapi.yml
  format: yaml
  label: Replicate Owner API
  slug: replicate-owner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-owner-api-openapi.yml
- filename: replicate-predictions-api-openapi.yml
  format: yaml
  label: Replicate Predictions API
  slug: replicate-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-predictions-api-openapi.yml
- filename: replicate-secrets-api-openapi.yml
  format: yaml
  label: Replicate Secrets API
  slug: replicate-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-secrets-api-openapi.yml
- filename: replicate-slug-api-openapi.yml
  format: yaml
  label: Replicate Slug API
  slug: replicate-slug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-slug-api-openapi.yml
- filename: replicate-training-api-openapi.yml
  format: yaml
  label: Replicate Training API
  slug: replicate-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-training-api-openapi.yml
- filename: replicate-trainings-api-openapi.yml
  format: yaml
  label: Replicate Trainings API
  slug: replicate-trainings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-trainings-api-openapi.yml
- filename: replicate-version-api-openapi.yml
  format: yaml
  label: Replicate Version API
  slug: replicate-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-version-api-openapi.yml
- filename: replicate-webhooks-api-openapi.yml
  format: yaml
  label: Replicate Webhooks API
  slug: replicate-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Replicate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replicate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Replicate
provider_slug: replicate
scheme_count: 1
schemes:
- bearerFormat: 'All API requests must include a valid API token in the `Authorization` request header. The token must be prefixed by "Bearer", followed by a space and the token value.

    Example: `Authorization: Bearer r8_Hw***********************************`

    Find your tokens at https://replicate.com/account/api-tokens

    '
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/replicate-openapi.yml
  type: http
slug: replicate-authentication
source_filename: replicate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/replicate-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: |\n    All API requests must include a valid API token in the `Authorization` request header. The token must be prefixed by \"Bearer\", followed by a space and the token value.\n    Example: `Authorization: Bearer r8_Hw***********************************`\n    Find your tokens at https://replicate.com/account/api-tokens\n  sources:\n  - openapi/replicate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/authentication/replicate-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Machine-Learning
- Image-Generation
- Language Models
- Model Deployment
---
