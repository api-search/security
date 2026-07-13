---
api_key_in: []
api_specs:
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Web Endpoints API
  slug: beam-cloud-web-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Task Queues API
  slug: beam-cloud-task-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Tasks Management API
  slug: beam-cloud-tasks-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Sandboxes and Volumes API
  slug: beam-cloud-sandboxes-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Beam Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beam secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Beam
provider_slug: beam-cloud
scheme_count: 1
schemes:
- description: 'Beam API token passed as `Authorization: Bearer <TOKEN>`. Generate tokens in the Beam dashboard or with the Beam CLI.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/beam-cloud-openapi.yml
  type: http
slug: beam-cloud-authentication
source_filename: beam-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/beam-cloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Beam API token passed as `Authorization: Bearer <TOKEN>`. Generate tokens in\n    the Beam dashboard or with the Beam CLI.'\n  sources:\n  - openapi/beam-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/authentication/beam-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Serverless
- GPU
- Python
- Inference
- Containers
---
