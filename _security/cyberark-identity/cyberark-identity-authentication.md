---
api_key_in: []
api_specs:
- filename: cyberark-identity-openapi.yml
  format: yaml
  label: CyberArk Identity API
  slug: identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/openapi/cyberark-identity-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cyberark Identity Authentication
name_suffix: Authentication
oauth_flows: []
overview: CyberArk Identity secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CyberArk Identity
provider_slug: cyberark-identity
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 / OIDC bearer token issued by /OAuth2/Token/{appId}.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cyberark-identity-openapi.yml
  type: http
- description: HTTP Basic with OAuth client credentials, used only for /OAuth2/Token/{appId}.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cyberark-identity-openapi.yml
  type: http
slug: cyberark-identity-authentication
source_filename: cyberark-identity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cyberark-identity-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 / OIDC bearer token issued by /OAuth2/Token/{appId}.\n  sources:\n  - openapi/cyberark-identity-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with OAuth client credentials, used only for /OAuth2/Token/{appId}.\n  sources:\n  - openapi/cyberark-identity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/authentication/cyberark-identity-authentication.yml
summary_line: http · 2 schemes
tags:
- Identity
- Access Management
- IAM
- Single Sign-On
- SSO
- Multi-Factor Authentication
- OAuth
- Zero Trust
---
