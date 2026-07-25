---
api_key_in: []
api_specs:
- filename: modal-com-apps-api-openapi.yml
  format: yaml
  label: Modal Apps API
  slug: modal-com-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-apps-api-openapi.yml
- filename: modal-com-dicts-api-openapi.yml
  format: yaml
  label: Modal Dicts API
  slug: modal-com-dicts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-dicts-api-openapi.yml
- filename: modal-com-environments-api-openapi.yml
  format: yaml
  label: Modal Environments API
  slug: modal-com-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-environments-api-openapi.yml
- filename: modal-com-execution-api-openapi.yml
  format: yaml
  label: Modal Execution API
  slug: modal-com-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-execution-api-openapi.yml
- filename: modal-com-files-api-openapi.yml
  format: yaml
  label: Modal Files API
  slug: modal-com-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-files-api-openapi.yml
- filename: modal-com-filesystem-api-openapi.yml
  format: yaml
  label: Modal Filesystem API
  slug: modal-com-filesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-filesystem-api-openapi.yml
- filename: modal-com-functions-api-openapi.yml
  format: yaml
  label: Modal Functions API
  slug: modal-com-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-functions-api-openapi.yml
- filename: modal-com-images-api-openapi.yml
  format: yaml
  label: Modal Images API
  slug: modal-com-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-images-api-openapi.yml
- filename: modal-com-invocations-api-openapi.yml
  format: yaml
  label: Modal Invocations API
  slug: modal-com-invocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-invocations-api-openapi.yml
- filename: modal-com-queues-api-openapi.yml
  format: yaml
  label: Modal Queues API
  slug: modal-com-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-queues-api-openapi.yml
- filename: modal-com-sandboxes-api-openapi.yml
  format: yaml
  label: Modal Sandboxes API
  slug: modal-com-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-sandboxes-api-openapi.yml
- filename: modal-com-schedules-api-openapi.yml
  format: yaml
  label: Modal Schedules API
  slug: modal-com-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-schedules-api-openapi.yml
- filename: modal-com-secrets-api-openapi.yml
  format: yaml
  label: Modal Secrets API
  slug: modal-com-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-secrets-api-openapi.yml
- filename: modal-com-tokens-api-openapi.yml
  format: yaml
  label: Modal Tokens API
  slug: modal-com-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-tokens-api-openapi.yml
- filename: modal-com-volumes-api-openapi.yml
  format: yaml
  label: Modal Volumes API
  slug: modal-com-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-volumes-api-openapi.yml
- filename: modal-com-webendpoints-api-openapi.yml
  format: yaml
  label: Modal WebEndpoints API
  slug: modal-com-webendpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-webendpoints-api-openapi.yml
- filename: modal-com-workspaces-api-openapi.yml
  format: yaml
  label: Modal Workspaces API
  slug: modal-com-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-com-workspaces-api-openapi.yml
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
