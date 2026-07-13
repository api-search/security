---
api_key_in: []
api_specs:
- filename: open-source
  format: yaml
  label: Kestra Flows API
  slug: flows-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Executions API
  slug: executions-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Namespaces API
  slug: namespaces-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Key-Value Store API
  slug: kv-store-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Namespace Files API
  slug: namespace-files-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kestra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kestra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kestra
provider_slug: kestra
scheme_count: 1
schemes:
- description: Optional HTTP basic authentication for self-hosted Kestra instances.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/kestra-openapi.yml
  type: http
slug: kestra-authentication
source_filename: kestra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kestra-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Optional HTTP basic authentication for self-hosted Kestra instances.\n  sources:\n  - openapi/kestra-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kestra/refs/heads/main/authentication/kestra-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- Data Pipelines
- Event-Driven
- Orchestration
- Workflows
---
