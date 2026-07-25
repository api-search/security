---
api_key_in: []
api_specs:
- filename: codesandbox-meta-api-openapi.yml
  format: yaml
  label: CodeSandbox meta API
  slug: codesandbox-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/openapi/codesandbox-meta-api-openapi.yml
- filename: codesandbox-preview-host-api-openapi.yml
  format: yaml
  label: CodeSandbox preview_host API
  slug: codesandbox-preview-host-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/openapi/codesandbox-preview-host-api-openapi.yml
- filename: codesandbox-preview-token-api-openapi.yml
  format: yaml
  label: CodeSandbox preview_token API
  slug: codesandbox-preview-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/openapi/codesandbox-preview-token-api-openapi.yml
- filename: codesandbox-sandbox-api-openapi.yml
  format: yaml
  label: CodeSandbox sandbox API
  slug: codesandbox-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/openapi/codesandbox-sandbox-api-openapi.yml
- filename: codesandbox-templates-api-openapi.yml
  format: yaml
  label: CodeSandbox templates API
  slug: codesandbox-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/openapi/codesandbox-templates-api-openapi.yml
- filename: codesandbox-token-api-openapi.yml
  format: yaml
  label: CodeSandbox token API
  slug: codesandbox-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/openapi/codesandbox-token-api-openapi.yml
- filename: codesandbox-vm-api-openapi.yml
  format: yaml
  label: CodeSandbox vm API
  slug: codesandbox-vm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/openapi/codesandbox-vm-api-openapi.yml
- filename: codesandbox-workspace-api-openapi.yml
  format: yaml
  label: CodeSandbox workspace API
  slug: codesandbox-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/openapi/codesandbox-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Codesandbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeSandbox secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CodeSandbox
provider_slug: codesandbox
scheme_count: 1
schemes:
- name: authorization
  scheme: bearer
  sources:
  - openapi/codesandbox-sdk-openapi.yml
  type: http
slug: codesandbox-authentication
source_filename: codesandbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codesandbox-sdk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/codesandbox-sdk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/authentication/codesandbox-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Tools
- Cloud IDE
- Code Sandboxes
- Browser Development
- AI Sandboxes
- Code Embedding
---
