---
api_key_in: []
api_specs:
- filename: temporal-io-cluster-api-openapi.yml
  format: yaml
  label: Temporal Cluster API
  slug: temporal-io-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/openapi/temporal-io-cluster-api-openapi.yml
- filename: temporal-io-namespaces-api-openapi.yml
  format: yaml
  label: Temporal Namespaces API
  slug: temporal-io-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/openapi/temporal-io-namespaces-api-openapi.yml
- filename: temporal-io-workflow-lifecycle-api-openapi.yml
  format: yaml
  label: Temporal Workflow Lifecycle API
  slug: temporal-io-workflow-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/openapi/temporal-io-workflow-lifecycle-api-openapi.yml
- filename: temporal-io-workflow-messaging-api-openapi.yml
  format: yaml
  label: Temporal Workflow Messaging API
  slug: temporal-io-workflow-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/openapi/temporal-io-workflow-messaging-api-openapi.yml
- filename: temporal-io-workflows-api-openapi.yml
  format: yaml
  label: Temporal Workflows API
  slug: temporal-io-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/openapi/temporal-io-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Temporal Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Temporal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Temporal
provider_slug: temporal-io
scheme_count: 1
schemes:
- description: 'Bearer API key. On Temporal Cloud, pass an API key as `Authorization: Bearer <api-key>`. Self-hosted deployments may use mTLS instead. Requests are scoped to the namespace in the path.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/temporal-io-openapi.yml
  type: http
slug: temporal-io-authentication
source_filename: temporal-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/temporal-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer API key. On Temporal Cloud, pass an API key as `Authorization: Bearer\n    <api-key>`. Self-hosted deployments may use mTLS instead. Requests are scoped to the namespace\n    in the path.'\n  sources:\n  - openapi/temporal-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/authentication/temporal-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Durable Execution
- Workflow Orchestration
- gRPC
- Workflows
- Open Source
- Temporal Cloud
---
