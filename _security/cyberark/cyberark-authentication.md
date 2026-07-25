---
api_key_in: []
api_specs:
- filename: cyberark-authentication-api-openapi.yml
  format: yaml
  label: CyberArk Authentication API
  slug: cyberark-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/openapi/cyberark-authentication-api-openapi.yml
- filename: cyberark-health-api-openapi.yml
  format: yaml
  label: CyberArk Health API
  slug: cyberark-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/openapi/cyberark-health-api-openapi.yml
- filename: cyberark-policies-api-openapi.yml
  format: yaml
  label: CyberArk Policies API
  slug: cyberark-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/openapi/cyberark-policies-api-openapi.yml
- filename: cyberark-publickeys-api-openapi.yml
  format: yaml
  label: CyberArk PublicKeys API
  slug: cyberark-publickeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/openapi/cyberark-publickeys-api-openapi.yml
- filename: cyberark-resources-api-openapi.yml
  format: yaml
  label: CyberArk Resources API
  slug: cyberark-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/openapi/cyberark-resources-api-openapi.yml
- filename: cyberark-roles-api-openapi.yml
  format: yaml
  label: CyberArk Roles API
  slug: cyberark-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/openapi/cyberark-roles-api-openapi.yml
- filename: cyberark-secrets-api-openapi.yml
  format: yaml
  label: CyberArk Secrets API
  slug: cyberark-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/openapi/cyberark-secrets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cyberark Authentication
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/authentication/cyberark-authentication.yml
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
- PAM
- Privileged Access
- Privileged Access Management
- Secrets Management
- Session Management
- SSO
- Vault
- Zero Trust
---
