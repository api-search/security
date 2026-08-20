---
api_key_in: []
api_specs:
- filename: aqua-security-authentication-api-openapi.yml
  format: yaml
  label: Aqua Security Authentication API
  slug: aqua-security-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/openapi/aqua-security-authentication-api-openapi.yml
- filename: aqua-security-containers-api-openapi.yml
  format: yaml
  label: Aqua Security Containers API
  slug: aqua-security-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/openapi/aqua-security-containers-api-openapi.yml
- filename: aqua-security-images-api-openapi.yml
  format: yaml
  label: Aqua Security Images API
  slug: aqua-security-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/openapi/aqua-security-images-api-openapi.yml
- filename: aqua-security-policies-api-openapi.yml
  format: yaml
  label: Aqua Security Policies API
  slug: aqua-security-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/openapi/aqua-security-policies-api-openapi.yml
- filename: aqua-security-registries-api-openapi.yml
  format: yaml
  label: Aqua Security Registries API
  slug: aqua-security-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/openapi/aqua-security-registries-api-openapi.yml
- filename: aqua-security-users-api-openapi.yml
  format: yaml
  label: Aqua Security Users API
  slug: aqua-security-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/openapi/aqua-security-users-api-openapi.yml
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
- Cloud-Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
---
