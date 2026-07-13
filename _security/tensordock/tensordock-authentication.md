---
api_key_in: []
api_specs:
- filename: tensordock-marketplace-api-openapi.yml
  format: yaml
  label: TensorDock Marketplace API
  slug: tensordock-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-marketplace-api-openapi.yml
- filename: tensordock-instances-api-openapi.yml
  format: yaml
  label: TensorDock Instances API
  slug: tensordock-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-instances-api-openapi.yml
- filename: tensordock-secrets-api-openapi.yml
  format: yaml
  label: TensorDock Secrets API
  slug: tensordock-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-secrets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tensordock Authentication
name_suffix: Authentication
oauth_flows: []
overview: TensorDock secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TensorDock
provider_slug: tensordock
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'Bearer token authentication. Generate API tokens at

    https://dashboard.tensordock.com/api. Send the token in the

    `Authorization: Bearer <token>` header.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tensordock-instances-api-openapi.yml
  - openapi/tensordock-secrets-api-openapi.yml
  type: http
slug: tensordock-authentication
source_filename: tensordock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tensordock-instances-api-openapi.yml, openapi/tensordock-secrets-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: |-\n    Bearer token authentication. Generate API tokens at\n    https://dashboard.tensordock.com/api. Send the token in the\n    `Authorization: Bearer <token>` header.\n  sources:\n  - openapi/tensordock-instances-api-openapi.yml\n  - openapi/tensordock-secrets-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/authentication/tensordock-authentication.yml
summary_line: http · 1 scheme
tags:
- GPU
- Cloud
- Marketplace
- Compute
- Virtual Machines
- AI
- Machine Learning
- Bare Metal
- Spot Instances
- Containers
---
