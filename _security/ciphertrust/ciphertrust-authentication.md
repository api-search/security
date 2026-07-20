---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ciphertrust Authentication
name_suffix: Authentication
oauth_flows: []
overview: CipherTrust secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CipherTrust
provider_slug: ciphertrust
scheme_count: 1
schemes:
- bearer_format: JWT
  description: 'Clients POST credentials (or a refresh token) to /api/v1/auth/tokens to obtain a short-lived JWT access token, then send it as `Authorization: Bearer <jwt>` on subsequent /api/v1 requests. Grant types include password (username/password), refresh_token, and client_credentials for registered clients. Optional two-factor and external identity-provider (LDAP/OIDC) backed logins are supported.'
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  - github.com/ThalesGroup/terraform-provider-ciphertrust
  type: http
slug: ciphertrust-authentication
source_filename: ciphertrust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs-cybersec.thalesgroup.com/bundle/latest-cdsp-cm/page/reference/index.html\ndocs: https://docs-cybersec.thalesgroup.com/bundle/latest-cdsp-cm/page/reference/index.html\nsummary:\n  types: [http]\n  http_scheme: bearer\n  bearer_format: JWT\n  token_endpoint: POST /api/v1/auth/tokens\n  notes: >-\n    No public OpenAPI is published, so this profile is captured from the CipherTrust\n    Manager API reference and the official Terraform/Ansible clients rather than\n    derived from a spec. The API is served per CipherTrust Manager deployment.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Clients POST credentials (or a refresh token) to /api/v1/auth/tokens to obtain\n    a short-lived JWT access token, then send it as `Authorization: Bearer <jwt>`\n    on subsequent /api/v1 requests. Grant types include password (username/password),\n    refresh_token, and\
  \ client_credentials for registered clients. Optional\n    two-factor and external identity-provider (LDAP/OIDC) backed logins are supported.\n  sources: [docs, github.com/ThalesGroup/terraform-provider-ciphertrust]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciphertrust/refs/heads/main/authentication/ciphertrust-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Encryption
- Key Management
- Secrets Management
- Data Protection
- Cryptography
- Tokenization
- Compliance
- KMIP
---
