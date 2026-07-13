---
api_key_in: []
api_specs:
- filename: materialize-openapi.yml
  format: yaml
  label: Materialize HTTP API
  slug: materialize-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materialize/refs/heads/main/openapi/materialize-openapi.yml
- filename: materialize-asyncapi.yml
  format: yaml
  label: Materialize Streaming Sources and Sinks (AsyncAPI)
  slug: materialize-streaming-asyncapi
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/materialize/refs/heads/main/asyncapi/materialize-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Materialize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Materialize secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Materialize
provider_slug: materialize
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication using your Materialize email as the username

    and an app password as the password.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/materialize-openapi.yml
  type: http
slug: materialize-authentication
source_filename: materialize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/materialize-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic authentication using your Materialize email as the username\n    and an app password as the password.\n  sources:\n  - openapi/materialize-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/materialize/refs/heads/main/authentication/materialize-authentication.yml
summary_line: http · 1 scheme
tags:
- Streaming
- Data Warehouse
- SQL
- Real-Time
- PostgreSQL Compatible
---
