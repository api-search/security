---
api_key_in: []
api_specs:
- filename: github-container-registry-organization-packages-api-openapi.yml
  format: yaml
  label: GitHub Container Registry Organization Packages API
  slug: github-container-registry-organization-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-container-registry/refs/heads/main/openapi/github-container-registry-organization-packages-api-openapi.yml
- filename: github-container-registry-user-namespace-packages-api-openapi.yml
  format: yaml
  label: GitHub Container Registry User Namespace Packages API
  slug: github-container-registry-user-namespace-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-container-registry/refs/heads/main/openapi/github-container-registry-user-namespace-packages-api-openapi.yml
- filename: github-container-registry-user-packages-api-openapi.yml
  format: yaml
  label: GitHub Container Registry User Packages API
  slug: github-container-registry-user-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-container-registry/refs/heads/main/openapi/github-container-registry-user-packages-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Github Container Registry Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitHub Container Registry secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GitHub Container Registry
provider_slug: github-container-registry
scheme_count: 1
schemes:
- bearerFormat: token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/github-container-registry-openapi.yml
  type: http
slug: github-container-registry-authentication
source_filename: github-container-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/github-container-registry-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  sources:\n  - openapi/github-container-registry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-container-registry/refs/heads/main/authentication/github-container-registry-authentication.yml
summary_line: http · 1 scheme
tags:
- Container Images
- Containers
- GitHub
- Packages
- Registry
---
