---
api_key_in: []
api_specs:
- filename: login-gov-oidc-openapi.yml
  format: yaml
  label: Login.gov OpenID Connect API
  slug: login-gov-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-oidc-openapi.yml
- filename: login-gov-saml-openapi.yml
  format: yaml
  label: Login.gov SAML 2.0 API
  slug: login-gov-saml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-saml-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Login Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Login.gov secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Login.gov
provider_slug: login-gov
scheme_count: 1
schemes:
- bearerFormat: opaque
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/login-gov-oidc-openapi.yml
  type: http
slug: login-gov-authentication
source_filename: login-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/login-gov-oidc-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  sources:\n  - openapi/login-gov-oidc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/authentication/login-gov-authentication.yml
summary_line: http · 1 scheme
tags:
- Government
- Federal
- GSA
- Identity
- Authentication
- SSO
- OIDC
- SAML
- IAL2
- AAL2
---
