---
anonymous_access: false
api_key_in: []
api_specs:
- filename: guestgraph-io-operations-api-openapi.yml
  format: yaml
  label: guestgraph-io Operations API
  slug: guestgraph-io-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guestgraph-io/openapi/guestgraph-io-operations-api-openapi.yml
- filename: guestgraph-io-webhook-api-openapi.yml
  format: yaml
  label: guestgraph-io Webhook API
  slug: guestgraph-io-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guestgraph-io/openapi/guestgraph-io-webhook-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: guestgraph-io Authentication
name_suffix: Authentication
oauth_flows: []
overview: guestgraph-io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: guestgraph-io
provider_slug: guestgraph-io
scheme_count: 1
schemes:
- name: OpsToken
  scheme: bearer
  sources:
  - openapi/guestgraph-io-apaleo-openapi.yml
  type: http
slug: guestgraph-io-authentication
source_filename: guestgraph-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/guestgraph-io-apaleo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: OpsToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/guestgraph-io-apaleo-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/guestgraph-io/authentication/guestgraph-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity
- Guest Data
- Hotels
- Open Source
- Graph
---
