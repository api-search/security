---
api_key_in:
- header
api_specs:
- filename: portainer-openapi.yml
  format: yaml
  label: Portainer
  slug: portainer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portainer/refs/heads/main/openapi/portainer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Portainer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Portainer secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Portainer
provider_slug: portainer
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/portainer-openapi.yml
  type: apiKey
- in: header
  name: jwt
  parameter: Authorization
  sources:
  - openapi/portainer-openapi.yml
  type: apiKey
slug: portainer-authentication
source_filename: portainer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/portainer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/portainer-openapi.yml\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/portainer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portainer/refs/heads/main/authentication/portainer-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Container Management
- Containers
- Docker
- Kubernetes
---
