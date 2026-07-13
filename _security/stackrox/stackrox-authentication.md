---
api_key_in:
- header
api_specs:
- filename: stackrox-openapi.yml
  format: yaml
  label: StackRox API
  slug: stackrox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackrox/refs/heads/main/openapi/stackrox-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stackrox Authentication
name_suffix: Authentication
oauth_flows: []
overview: StackRox secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StackRox
provider_slug: stackrox
scheme_count: 1
schemes:
- description: 'StackRox API token. Format: Bearer {token}'
  in: header
  name: ApiToken
  parameter: Authorization
  sources:
  - openapi/stackrox-openapi.yml
  type: apiKey
slug: stackrox-authentication
source_filename: stackrox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stackrox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'StackRox API token. Format: Bearer {token}'\n  sources:\n  - openapi/stackrox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackrox/refs/heads/main/authentication/stackrox-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Container Security
- Kubernetes
- Open Source
- Runtime Protection
- Security
---
