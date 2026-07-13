---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Speakeasy
  slug: speakeasy
  spec_type: OpenAPI
  url: https://www.speakeasy.com/openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Speakeasy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Speakeasy secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Speakeasy
provider_slug: speakeasy
scheme_count: 3
schemes:
- description: The API Key for the workspace
  in: header
  name: APIKey
  parameter: x-api-key
  sources:
  - openapi/speakeasy-openapi.yml
  type: apiKey
- description: The API Key for the workspace
  in: header
  name: WorkspaceIdentifier
  parameter: x-workspace-identifier
  sources:
  - openapi/speakeasy-openapi.yml
  type: apiKey
- description: The Bearer token for the workspace
  name: Bearer
  scheme: bearer
  sources:
  - openapi/speakeasy-openapi.yml
  type: http
slug: speakeasy-authentication
source_filename: speakeasy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/speakeasy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The API Key for the workspace\n  sources:\n  - openapi/speakeasy-openapi.yml\n- name: WorkspaceIdentifier\n  type: apiKey\n  in: header\n  parameter: x-workspace-identifier\n  description: The API Key for the workspace\n  sources:\n  - openapi/speakeasy-openapi.yml\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: The Bearer token for the workspace\n  sources:\n  - openapi/speakeasy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/authentication/speakeasy-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- AI
- Documentation
- MCP
- Platform
- SDKs
- Terraform
- Testing
---
