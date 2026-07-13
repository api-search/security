---
api_key_in:
- header
api_specs:
- filename: dokploy-openapi.yml
  format: yaml
  label: Dokploy
  slug: dokploy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dokploy/refs/heads/main/openapi/dokploy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dokploy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dokploy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dokploy
provider_slug: dokploy
scheme_count: 1
schemes:
- description: API key authentication. Generate an API key from your Dokploy dashboard under Settings > API Keys.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/dokploy-openapi.yml
  type: apiKey
slug: dokploy-authentication
source_filename: dokploy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dokploy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key authentication. Generate an API key from your Dokploy dashboard under\n    Settings > API Keys.\n  sources:\n  - openapi/dokploy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dokploy/refs/heads/main/authentication/dokploy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- PaaS
- Self-Hosted
- Open Source
- Docker
- Docker Swarm
- Deployment
- Traefik
- Databases
---
