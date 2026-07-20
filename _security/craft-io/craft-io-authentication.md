---
api_key_in:
- header
api_specs:
- filename: docs
  format: yaml
  label: Craft.io Workspace API
  slug: craftio-workspace-api
  spec_type: OpenAPI
  url: https://api.craft.io/docs
- filename: docs
  format: yaml
  label: Craft.io Portfolio API
  slug: craftio-portfolio-api
  spec_type: OpenAPI
  url: https://api.craft.io/docs
- filename: docs
  format: yaml
  label: Craft.io Feedback Portal API
  slug: craftio-feedback-portal-api
  spec_type: OpenAPI
  url: https://api.craft.io/docs
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Craft Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Craft.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Craft.io
provider_slug: craft-io
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/craft-io-feedback-openapi.yml
  - openapi/craft-io-portfolio-openapi.yml
  - openapi/craft-io-workspace-openapi.yml
  type: apiKey
slug: craft-io-authentication
source_filename: craft-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/craft-io-feedback-openapi.yml, openapi/craft-io-portfolio-openapi.yml, openapi/craft-io-workspace-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/craft-io-feedback-openapi.yml\n  - openapi/craft-io-portfolio-openapi.yml\n  - openapi/craft-io-workspace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craft-io/refs/heads/main/authentication/craft-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Product Management
- Roadmaps
- OKRs
- Backlog
- Feedback
- Portfolio
- Specifications
---
