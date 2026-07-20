---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Casdoor REST API
  slug: casdoor-rest-api
  spec_type: OpenAPI
  url: https://door.casdoor.com/swagger/
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
- OAuth
- OIDC
- Open Source
- Passkeys
- SAML
- SCIM
- Single Sign-On
- SSO
- WebAuthn
---
