---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Keycorp Authentication
name_suffix: Authentication
oauth_flows: []
overview: KeyCorp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KeyCorp
provider_slug: keycorp
scheme_count: 1
schemes:
- description: 'Bearer token issued by KeyBank''s OAuth flow for partner applications.

    Example: `Authorization: Bearer [example key]`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/keycorp-openapi.yml
  type: http
slug: keycorp-authentication
source_filename: keycorp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keycorp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token issued by KeyBank's OAuth flow for partner applications.\n    Example: `Authorization: Bearer [example key]`.\n  sources:\n  - openapi/keycorp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/authentication/keycorp-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Commercial Banking
- Financial Services
- Fortune 500
- Payments
---
