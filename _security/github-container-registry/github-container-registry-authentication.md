---
anonymous_access: false
api_key_in: []
api_specs:
- filename: github-container-registry-merge-queue-api-openapi.yml
  format: yaml
  label: GitHub Container Registry Merge Queue API
  slug: github-container-registry-merge-queue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-container-registry/openapi/github-container-registry-merge-queue-api-openapi.yml
- filename: github-container-registry-packages-api-openapi.yml
  format: yaml
  label: GitHub Container Registry Packages API
  slug: github-container-registry-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-container-registry/openapi/github-container-registry-packages-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GitHub Container Registry Authentication
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
  - openapi/_superseded/github-container-registry-organization-packages-api-openapi.yml
  - openapi/_superseded/github-container-registry-user-namespace-packages-api-openapi.yml
  - openapi/_superseded/github-container-registry-user-packages-api-openapi.yml
  type: http
slug: github-container-registry-authentication
source_filename: github-container-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/github-container-registry-organization-packages-api-openapi.yml, openapi/_superseded/github-container-registry-user-namespace-packages-api-openapi.yml,\n  openapi/_superseded/github-container-registry-user-packages-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  sources:\n  - openapi/_superseded/github-container-registry-organization-packages-api-openapi.yml\n  - openapi/_superseded/github-container-registry-user-namespace-packages-api-openapi.yml\n  - openapi/_superseded/github-container-registry-user-packages-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/github-container-registry/authentication/github-container-registry-authentication.yml
summary_line: http · 1 scheme
tags:
- Container Images
- Containers
- GitHub
- Packages
- Registry
- OCI
- Docker
---
