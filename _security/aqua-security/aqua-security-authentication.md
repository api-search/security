---
api_key_in: []
api_specs:
- filename: aqua-security-api.yaml
  format: yaml
  label: Aqua Security
  slug: aqua-security
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/openapi/aqua-security-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aqua Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aqua Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aqua Security
provider_slug: aqua-security
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained from the /v1/login endpoint
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/aqua-security-api.yaml
  type: http
slug: aqua-security-authentication
source_filename: aqua-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aqua-security-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from the /v1/login endpoint\n  sources:\n  - openapi/aqua-security-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/authentication/aqua-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
---
