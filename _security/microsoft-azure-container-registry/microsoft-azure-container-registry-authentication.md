---
api_key_in: []
api_specs:
- filename: microsoft-azure-container-registry-openapi.yml
  format: yaml
  label: Azure Container Registry API
  slug: azure-container-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-container-registry/refs/heads/main/openapi/microsoft-azure-container-registry-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Container Registry Authentication
name_suffix: Authentication
oauth_flows: []
overview: microsoft-azure-container-registry secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: microsoft-azure-container-registry
provider_slug: microsoft-azure-container-registry
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-azure-container-registry-openapi.yml
  type: http
slug: microsoft-azure-container-registry-authentication
source_filename: microsoft-azure-container-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-container-registry-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/microsoft-azure-container-registry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-container-registry/refs/heads/main/authentication/microsoft-azure-container-registry-authentication.yml
summary_line: http · 1 scheme
tags: []
---
