---
api_key_in: []
api_specs:
- filename: scalable-software-and-systems-openapi.yml
  format: yaml
  label: Backstage Software Catalog API
  slug: backstage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-software-and-systems/refs/heads/main/openapi/scalable-software-and-systems-openapi.yml
- filename: openapi.yml
  format: yaml
  label: Temporal API
  slug: temporal
  spec_type: OpenAPI
  url: https://github.com/temporalio/api/blob/master/openapi/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scalable Software And Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalable Software and Systems secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalable Software and Systems
provider_slug: scalable-software-and-systems
scheme_count: 1
schemes:
- bearerFormat: BackstageToken
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/scalable-software-and-systems-openapi.yml
  type: http
slug: scalable-software-and-systems-authentication
source_filename: scalable-software-and-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalable-software-and-systems-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: BackstageToken\n  sources:\n  - openapi/scalable-software-and-systems-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-software-and-systems/refs/heads/main/authentication/scalable-software-and-systems-authentication.yml
summary_line: http · 1 scheme
tags:
- API First
- Architecture Patterns
- CQRS
- Distributed Systems
- Enterprise
- Event Driven
- Microservices
- Scalable Architecture
- Software Engineering
- Systems Design
---
