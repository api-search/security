---
api_key_in: []
api_specs:
- filename: open-api-spec.yaml
  format: yaml
  label: WorkOS API
  slug: workos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/workos/openapi-spec/main/spec/open-api-spec.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workos Authentication
name_suffix: Authentication
oauth_flows: []
overview: WorkOS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WorkOS
provider_slug: workos
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Your WorkOS API key prefixed with `sk_`. Pass it as a Bearer token: `Authorization: Bearer sk_example_123456789`.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/workos-openapi.yml
  type: http
slug: workos-authentication
source_filename: workos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workos-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Your WorkOS API key prefixed with `sk_`. Pass it as a Bearer token: `Authorization:\n    Bearer sk_example_123456789`.'\n  sources:\n  - openapi/workos-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workos/refs/heads/main/authentication/workos-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Identity Provider
- SSO
- SAML
- OIDC
- SCIM
- Directory Sync
- Authorization
- FGA
- Audit Logs
- MFA
- B2B SaaS
- Agents
- MCP
---
