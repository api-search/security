---
api_key_in: []
api_specs:
- filename: modal-functions-openapi.yml
  format: yaml
  label: Modal Functions API
  slug: modal-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-functions-openapi.yml
- filename: modal-sandboxes-openapi.yml
  format: yaml
  label: Modal Sandboxes API
  slug: modal-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-sandboxes-openapi.yml
- filename: modal-volumes-openapi.yml
  format: yaml
  label: Modal Volumes API
  slug: modal-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-volumes-openapi.yml
- filename: modal-images-openapi.yml
  format: yaml
  label: Modal Images API
  slug: modal-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-images-openapi.yml
- filename: modal-secrets-openapi.yml
  format: yaml
  label: Modal Secrets API
  slug: modal-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-secrets-openapi.yml
- filename: modal-dicts-queues-openapi.yml
  format: yaml
  label: Modal Dicts and Queues API
  slug: modal-dicts-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-dicts-queues-openapi.yml
- filename: modal-schedules-openapi.yml
  format: yaml
  label: Modal Schedules API
  slug: modal-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-schedules-openapi.yml
- filename: modal-web-endpoints-openapi.yml
  format: yaml
  label: Modal Web Endpoints API
  slug: modal-web-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-web-endpoints-openapi.yml
- filename: modal-tokens-openapi.yml
  format: yaml
  label: Modal Tokens and Administration API
  slug: modal-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-tokens-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Modal Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Modal
provider_slug: modal
scheme_count: 1
schemes:
- name: ModalToken
  scheme: bearer
  sources:
  - openapi/modal-dicts-queues-openapi.yml
  - openapi/modal-functions-openapi.yml
  - openapi/modal-images-openapi.yml
  - openapi/modal-sandboxes-openapi.yml
  - openapi/modal-schedules-openapi.yml
  - openapi/modal-secrets-openapi.yml
  - openapi/modal-tokens-openapi.yml
  - openapi/modal-volumes-openapi.yml
  - openapi/modal-web-endpoints-openapi.yml
  type: http
slug: modal-com-authentication
source_filename: modal-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/modal-dicts-queues-openapi.yml, openapi/modal-functions-openapi.yml, openapi/modal-images-openapi.yml,\n  openapi/modal-sandboxes-openapi.yml, openapi/modal-schedules-openapi.yml, openapi/modal-secrets-openapi.yml,\n  openapi/modal-tokens-openapi.yml, openapi/modal-volumes-openapi.yml, openapi/modal-web-endpoints-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ModalToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/modal-dicts-queues-openapi.yml\n  - openapi/modal-functions-openapi.yml\n  - openapi/modal-images-openapi.yml\n  - openapi/modal-sandboxes-openapi.yml\n  - openapi/modal-schedules-openapi.yml\n  - openapi/modal-secrets-openapi.yml\n  - openapi/modal-tokens-openapi.yml\n  - openapi/modal-volumes-openapi.yml\n  - openapi/modal-web-endpoints-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/authentication/modal-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Serverless
- GPU
- Cloud Compute
- AI Infrastructure
- Sandboxes
- Inference
- Training
- Batch Processing
- Python
- TypeScript
- Go
---
