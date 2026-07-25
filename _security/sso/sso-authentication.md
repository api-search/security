---
api_key_in: []
api_specs:
- filename: sso-authentication-api-openapi.yml
  format: yaml
  label: SSO Authentication API
  slug: sso-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-authentication-api-openapi.yml
- filename: sso-authorization-api-openapi.yml
  format: yaml
  label: SSO Authorization API
  slug: sso-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-authorization-api-openapi.yml
- filename: sso-discovery-api-openapi.yml
  format: yaml
  label: SSO Discovery API
  slug: sso-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-discovery-api-openapi.yml
- filename: sso-keys-api-openapi.yml
  format: yaml
  label: SSO Keys API
  slug: sso-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-keys-api-openapi.yml
- filename: sso-logout-api-openapi.yml
  format: yaml
  label: SSO Logout API
  slug: sso-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-logout-api-openapi.yml
- filename: sso-metadata-api-openapi.yml
  format: yaml
  label: SSO Metadata API
  slug: sso-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-metadata-api-openapi.yml
- filename: sso-token-api-openapi.yml
  format: yaml
  label: SSO Token API
  slug: sso-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-token-api-openapi.yml
- filename: sso-user-info-api-openapi.yml
  format: yaml
  label: SSO User Info API
  slug: sso-user-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-user-info-api-openapi.yml
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
