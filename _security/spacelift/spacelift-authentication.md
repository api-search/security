---
api_key_in: []
api_specs:
- filename: spacelift-openapi.yml
  format: yaml
  label: Spacelift GraphQL API
  slug: spacelift-graphql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacelift/refs/heads/main/openapi/spacelift-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spacelift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spacelift secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spacelift
provider_slug: spacelift
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT bearer token obtained from the `apiKeyUser` or `oauthUser`

    mutation, or via `spacectl profile export-token`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/spacelift-openapi.yml
  type: http
slug: spacelift-authentication
source_filename: spacelift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spacelift-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT bearer token obtained from the `apiKeyUser` or `oauthUser`\n    mutation, or via `spacectl profile export-token`.\n  sources:\n  - openapi/spacelift-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacelift/refs/heads/main/authentication/spacelift-authentication.yml
summary_line: http · 1 scheme
tags:
- Infrastructure as Code
- FinOps
- DevOps
- Platform Engineering
- Terraform
- GitOps
---
