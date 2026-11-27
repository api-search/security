---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: CyberArk Authentication
name_suffix: Authentication
oauth_flows: []
overview: CyberArk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CyberArk
provider_slug: cyberark
scheme_count: 1
schemes:
- bearerFormat: ConjurAccessToken
  name: ConjurAuth
  scheme: bearer
  sources:
  - openapi/cyberark-conjur-openapi.yml
  type: http
slug: cyberark-authentication
source_filename: cyberark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cyberark-conjur-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ConjurAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ConjurAccessToken\n  sources:\n  - openapi/cyberark-conjur-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/cyberark/authentication/cyberark-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Cloud Security
- Conjur
- Credential Vault
- DevOps Secrets
- Endpoint Privilege Management
- Identity Security
- Machine Identity
- MFA
- OpenAPI
- Privileged Access Management
- Secrets Management
- Session Management
- SSO
- Vault
- Zero Trust
- Identity Federation
---
