---
api_key_in: []
api_specs:
- filename: login-gov-authentication-api-openapi.yml
  format: yaml
  label: Login.gov Authentication API
  slug: login-gov-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-authentication-api-openapi.yml
- filename: login-gov-authorization-api-openapi.yml
  format: yaml
  label: Login.gov Authorization API
  slug: login-gov-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-authorization-api-openapi.yml
- filename: login-gov-discovery-api-openapi.yml
  format: yaml
  label: Login.gov Discovery API
  slug: login-gov-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-discovery-api-openapi.yml
- filename: login-gov-logout-api-openapi.yml
  format: yaml
  label: Login.gov Logout API
  slug: login-gov-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-logout-api-openapi.yml
- filename: login-gov-metadata-api-openapi.yml
  format: yaml
  label: Login.gov Metadata API
  slug: login-gov-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-metadata-api-openapi.yml
- filename: login-gov-token-api-openapi.yml
  format: yaml
  label: Login.gov Token API
  slug: login-gov-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-token-api-openapi.yml
- filename: login-gov-userinfo-api-openapi.yml
  format: yaml
  label: Login.gov UserInfo API
  slug: login-gov-userinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-userinfo-api-openapi.yml
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
