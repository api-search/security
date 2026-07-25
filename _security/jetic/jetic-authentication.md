---
api_key_in: []
api_specs:
- filename: jetic-api-specifications-api-openapi.yml
  format: yaml
  label: Jetic API Specifications API
  slug: jetic-api-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-api-specifications-api-openapi.yml
- filename: jetic-clusters-api-openapi.yml
  format: yaml
  label: Jetic Clusters API
  slug: jetic-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-clusters-api-openapi.yml
- filename: jetic-deployments-api-openapi.yml
  format: yaml
  label: Jetic Deployments API
  slug: jetic-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-deployments-api-openapi.yml
- filename: jetic-integrations-api-openapi.yml
  format: yaml
  label: Jetic Integrations API
  slug: jetic-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-integrations-api-openapi.yml
- filename: jetic-monitoring-api-openapi.yml
  format: yaml
  label: Jetic Monitoring API
  slug: jetic-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-monitoring-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jetic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jetic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jetic
provider_slug: jetic
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained via the Jetic platform authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jetic-platform-openapi.yml
  type: http
slug: jetic-authentication
source_filename: jetic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jetic-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained via the Jetic platform authentication.\n  sources:\n  - openapi/jetic-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/authentication/jetic-authentication.yml
summary_line: http · 1 scheme
tags:
- Apache Camel
- Integrations
- iPaaS
- Pro-Code API Composition
---
