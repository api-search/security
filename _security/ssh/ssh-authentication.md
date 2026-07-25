---
api_key_in: []
api_specs:
- filename: ssh-authorized-keys-api-openapi.yml
  format: yaml
  label: SSH Authorized Keys API
  slug: ssh-authorized-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssh/refs/heads/main/openapi/ssh-authorized-keys-api-openapi.yml
- filename: ssh-certificates-api-openapi.yml
  format: yaml
  label: SSH Certificates API
  slug: ssh-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssh/refs/heads/main/openapi/ssh-certificates-api-openapi.yml
- filename: ssh-host-keys-api-openapi.yml
  format: yaml
  label: SSH Host Keys API
  slug: ssh-host-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssh/refs/heads/main/openapi/ssh-host-keys-api-openapi.yml
- filename: ssh-keys-api-openapi.yml
  format: yaml
  label: SSH Keys API
  slug: ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssh/refs/heads/main/openapi/ssh-keys-api-openapi.yml
- filename: ssh-known-hosts-api-openapi.yml
  format: yaml
  label: SSH Known Hosts API
  slug: ssh-known-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssh/refs/heads/main/openapi/ssh-known-hosts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ssh Authentication
name_suffix: Authentication
oauth_flows: []
overview: SSH secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SSH
provider_slug: ssh
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ssh-key-management-openapi.yml
  type: http
slug: ssh-authentication
source_filename: ssh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ssh-key-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ssh-key-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ssh/refs/heads/main/authentication/ssh-authentication.yml
summary_line: http · 1 scheme
tags:
- SSH
- Secure Shell
- Remote Access
- Cryptography
- Network Security
- System Administration
---
