---
api_key_in: []
api_specs:
- filename: smallstep-openapi-original.yml
  format: yaml
  label: Smallstep Platform API
  slug: smallstep-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallstep/refs/heads/main/openapi/smallstep-openapi-original.yml
auth_types:
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Smallstep Authentication
name_suffix: Authentication
oauth_flows: []
overview: SmallStep secures its APIs with http and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SmallStep
provider_slug: smallstep
scheme_count: 2
schemes:
- name: JWT
  scheme: bearer
  sources:
  - openapi/smallstep-openapi-original.yml
  type: http
- description: Use a client certificate issued by a trusted root to get short-lived bearer tokens with the step CLI.
  name: mtls
  sources:
  - openapi/smallstep-openapi-original.yml
  type: mutualTLS
slug: smallstep-authentication
source_filename: smallstep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/smallstep-openapi-original.yml\ndocs: https://smallstep.com/docs/platform/smallstep-api/\nnotes: >-\n  Global default is JWT bearer. Tokens are minted in the Smallstep UI (with selectable scopes and\n  validity period) or via `step api token create`, which exchanges a client certificate issued by a\n  configured trusted root for a short-lived (1 hour) bearer token — the mutual-TLS scheme applied to\n  POST /auth.\nsummary:\n  types:\n  - http\n  - mutualTLS\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/smallstep-openapi-original.yml\n- name: mtls\n  type: mutualTLS\n  description: Use a client certificate issued by a trusted root to get short-lived bearer tokens\n    with the step CLI.\n  sources:\n  - openapi/smallstep-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smallstep/refs/heads/main/authentication/smallstep-authentication.yml
summary_line: http/mutualTLS · 2 schemes
tags:
- Company
- Developer Tools
- Certificate Authority
- PKI
- Device Identity
- Zero Trust
- Certificate Management
- mTLS
- ACME
- SSH
- Security
---
