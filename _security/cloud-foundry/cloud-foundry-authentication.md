---
api_key_in: []
api_specs:
- filename: cloud-foundry-cloud-controller-api-v3-openapi.yml
  format: yaml
  label: Cloud Foundry Cloud Controller API v3
  slug: cloud-controller-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-cloud-controller-api-v3-openapi.yml
- filename: cloud-foundry-loggregator-asyncapi.yml
  format: yaml
  label: Cloud Foundry Loggregator
  slug: loggregator
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/asyncapi/cloud-foundry-loggregator-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloud Foundry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud Foundry secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloud Foundry
provider_slug: cloud-foundry
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloud-foundry-openapi.yml
  type: http
slug: cloud-foundry-authentication
source_filename: cloud-foundry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-foundry-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cloud-foundry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/authentication/cloud-foundry-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Foundry Foundation
- Containers
- Multi-Cloud
- Open Source
- PaaS
- Platform
---
