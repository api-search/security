---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Docker Hub API
  slug: docker-hub-api
  spec_type: OpenAPI
  url: https://docs.docker.com/reference/api/hub/latest/
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Docker Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Docker Hub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Docker Hub
provider_slug: docker-hub
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/docker-hub-openapi.yml
  type: http
slug: docker-hub-authentication
source_filename: docker-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docker-hub-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/docker-hub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/authentication/docker-hub-authentication.yml
summary_line: http · 1 scheme
tags:
- Containers
- DevOps
- Docker
- Registry
---
