---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coreweave-freshdesk-api-openapi.yml
  format: yaml
  label: CoreWeave Freshdesk API
  slug: coreweave-freshdesk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coreweave/openapi/coreweave-freshdesk-api-openapi.yml
- filename: coreweave-healthz-api-openapi.yml
  format: yaml
  label: CoreWeave Healthz API
  slug: coreweave-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coreweave/openapi/coreweave-healthz-api-openapi.yml
- filename: coreweave-reconcile-api-openapi.yml
  format: yaml
  label: CoreWeave Reconcile API
  slug: coreweave-reconcile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coreweave/openapi/coreweave-reconcile-api-openapi.yml
- filename: coreweave-webhooks-api-openapi.yml
  format: yaml
  label: CoreWeave Webhooks API
  slug: coreweave-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coreweave/openapi/coreweave-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: CoreWeave Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoreWeave secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CoreWeave
provider_slug: coreweave
scheme_count: 1
schemes:
- bearerFormat: API Access Token
  description: 'Provide a CoreWeave API access token using the `Authorization: Bearer

    {API_ACCESS_TOKEN}` header.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/coreweave-openapi.yml
  type: http
slug: coreweave-authentication
source_filename: coreweave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coreweave-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Access Token\n  description: |-\n    Provide a CoreWeave API access token using the `Authorization: Bearer\n    {API_ACCESS_TOKEN}` header.\n  sources:\n  - openapi/coreweave-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/coreweave/authentication/coreweave-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Cloud
- GPU
- HPC
- Inference
- Kubernetes
- Machine Learning
- Storage
- Data Center
---
