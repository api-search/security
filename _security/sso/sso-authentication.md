---
api_key_in: []
api_specs:
- filename: sso-saml-openapi.yml
  format: yaml
  label: SAML SSO Authentication API
  slug: saml-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-saml-openapi.yml
- filename: sso-oidc-openapi.yml
  format: yaml
  label: OpenID Connect (OIDC) Authentication API
  slug: oidc-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-oidc-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sso Authentication
name_suffix: Authentication
oauth_flows: []
overview: SSO secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SSO
provider_slug: sso
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer access token in Authorization header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sso-oidc-openapi.yml
  type: http
slug: sso-authentication
source_filename: sso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sso-oidc-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer access token in Authorization header\n  sources:\n  - openapi/sso-oidc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/authentication/sso-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Authorization
- Identity
- OAuth
- OIDC
- SAML
- Security
- Single Sign-On
- SSO
---
