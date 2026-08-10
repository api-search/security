---
api_key_in: []
api_specs:
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
- filename: tensordock-authorization-api-openapi.yml
  format: yaml
  label: TensorDock Authorization API
  slug: tensordock-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-authorization-api-openapi.yml
- filename: tensordock-billing-api-openapi.yml
  format: yaml
  label: TensorDock Billing API
  slug: tensordock-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-billing-api-openapi.yml
- filename: tensordock-containers-api-openapi.yml
  format: yaml
  label: TensorDock Containers API
  slug: tensordock-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-containers-api-openapi.yml
- filename: tensordock-hostnodes-api-openapi.yml
  format: yaml
  label: TensorDock Hostnodes API
  slug: tensordock-hostnodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-hostnodes-api-openapi.yml
- filename: tensordock-instant-vms-api-openapi.yml
  format: yaml
  label: TensorDock Instant VMs API
  slug: tensordock-instant-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-instant-vms-api-openapi.yml
- filename: tensordock-spot-api-openapi.yml
  format: yaml
  label: TensorDock Spot API
  slug: tensordock-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-spot-api-openapi.yml
- filename: tensordock-virtual-machines-api-openapi.yml
  format: yaml
  label: TensorDock Virtual Machines API
  slug: tensordock-virtual-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-virtual-machines-api-openapi.yml
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
