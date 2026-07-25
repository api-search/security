---
api_key_in: []
api_specs:
- filename: 1password-accounts-api-openapi.yml
  format: yaml
  label: 1Password Accounts API
  slug: 1password-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-accounts-api-openapi.yml
- filename: 1password-activity-api-openapi.yml
  format: yaml
  label: 1Password Activity API
  slug: 1password-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-activity-api-openapi.yml
- filename: 1password-audit-events-api-openapi.yml
  format: yaml
  label: 1Password Audit Events API
  slug: 1password-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-audit-events-api-openapi.yml
- filename: 1password-files-api-openapi.yml
  format: yaml
  label: 1Password Files API
  slug: 1password-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-files-api-openapi.yml
- filename: 1password-health-api-openapi.yml
  format: yaml
  label: 1Password Health API
  slug: 1password-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-health-api-openapi.yml
- filename: 1password-introspection-api-openapi.yml
  format: yaml
  label: 1Password Introspection API
  slug: 1password-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-introspection-api-openapi.yml
- filename: 1password-item-usages-api-openapi.yml
  format: yaml
  label: 1Password Item Usages API
  slug: 1password-item-usages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-item-usages-api-openapi.yml
- filename: 1password-items-api-openapi.yml
  format: yaml
  label: 1Password Items API
  slug: 1password-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-items-api-openapi.yml
- filename: 1password-metrics-api-openapi.yml
  format: yaml
  label: 1Password Metrics API
  slug: 1password-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-metrics-api-openapi.yml
- filename: 1password-sign-in-attempts-api-openapi.yml
  format: yaml
  label: 1Password Sign-In Attempts API
  slug: 1password-sign-in-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-sign-in-attempts-api-openapi.yml
- filename: 1password-vaults-api-openapi.yml
  format: yaml
  label: 1Password Vaults API
  slug: 1password-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-vaults-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 1Password Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1Password secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 1Password
provider_slug: 1password
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: A Connect server access token generated from 1Password. Each request must include this token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/1password-connect-openapi.yml
  - openapi/1password-events-openapi.yml
  - openapi/1password-partnership-openapi.yml
  type: http
slug: 1password-authentication
source_filename: 1password-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/1password-connect-openapi.yml, openapi/1password-events-openapi.yml, openapi/1password-partnership-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A Connect server access token generated from 1Password. Each request must include\n    this token in the Authorization header.\n  sources:\n  - openapi/1password-connect-openapi.yml\n  - openapi/1password-events-openapi.yml\n  - openapi/1password-partnership-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/authentication/1password-authentication.yml
summary_line: http · 1 scheme
tags:
- Password Manager
- Passwords
- Security
- Secrets
---
