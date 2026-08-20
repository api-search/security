---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Casdoor REST API
  slug: casdoor-rest-api
  spec_type: OpenAPI
  url: https://door.casdoor.com/swagger/
- filename: casdoor-applications-api-openapi.yml
  format: yaml
  label: Casdoor Applications API
  slug: casdoor-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casdoor/refs/heads/main/openapi/casdoor-applications-api-openapi.yml
- filename: casdoor-authentication-api-openapi.yml
  format: yaml
  label: Casdoor Authentication API
  slug: casdoor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casdoor/refs/heads/main/openapi/casdoor-authentication-api-openapi.yml
- filename: casdoor-oidc-api-openapi.yml
  format: yaml
  label: Casdoor OIDC API
  slug: casdoor-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casdoor/refs/heads/main/openapi/casdoor-oidc-api-openapi.yml
- filename: casdoor-organizations-api-openapi.yml
  format: yaml
  label: Casdoor Organizations API
  slug: casdoor-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casdoor/refs/heads/main/openapi/casdoor-organizations-api-openapi.yml
- filename: casdoor-permissions-api-openapi.yml
  format: yaml
  label: Casdoor Permissions API
  slug: casdoor-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casdoor/refs/heads/main/openapi/casdoor-permissions-api-openapi.yml
- filename: casdoor-roles-api-openapi.yml
  format: yaml
  label: Casdoor Roles API
  slug: casdoor-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casdoor/refs/heads/main/openapi/casdoor-roles-api-openapi.yml
- filename: casdoor-users-api-openapi.yml
  format: yaml
  label: Casdoor Users API
  slug: casdoor-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casdoor/refs/heads/main/openapi/casdoor-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Casdoor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Casdoor secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Casdoor
provider_slug: casdoor
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/casdoor-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/casdoor-openapi.yml
  type: http
slug: casdoor-authentication
source_filename: casdoor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/casdoor-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/casdoor-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/casdoor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casdoor/refs/heads/main/authentication/casdoor-authentication.yml
summary_line: http · 2 schemes
tags:
- Authentication
- Authorization
- IAM
- Identity
- LDAP
- MCP
- MFA
- OIDC
- Open-Source
- Passkeys
- SAML
- SCIM
- Single Sign-On
- SSO
- WebAuthn
---
